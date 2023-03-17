ошибок в работе операционной системы не выявлено

анализ логов выявил ошибки по дискам NVME

messages_localwarn.txt

2023-03-05T15:43:44.783047+03:00 xxidb3 kernel: [10795.893801][T31147] nvme nvme4: NVME-FC{4}: controller connectivity lost.
2023-03-05T16:08:24.416021+03:00 xxidb3 kernel: [  650.858079][  T522] nvme nvme1: NVME-FC{1}: transport association event: transport detected io error
2023-03-05T16:08:24.416030+03:00 xxidb3 kernel: [  650.858082][  T522] nvme nvme1: NVME-FC{1}: resetting controller
2023-03-05T16:08:24.456010+03:00 xxidb3 kernel: [  650.894379][  T522] nvme nvme1: NVME-FC{1}: error_recovery: Couldn't change state to CONNECTING

судя по логам, NVME диски подключены через внешнее устройство-накопитель и есть проблемы с драйвером 

hardware.txt

<3>[  803.586639][  T524] nvme nvme4: NVME-FC{4}: error_recovery: Couldn't change state to CONNECTING
<6>[  803.586650][ T7049] nvme nvme4: NVME-FC{4}: create association : host wwpn 0x100008f1eabf3dbd  rport wwpn 0x20112811eceddcf7: NQN "nqn.2014-08.org.nvmexpress.discovery"
<3>[  803.586768][ T7049] nvme nvme4: Connect command failed: host path error

дальнейший анализ показал, что ядро ОС модифицировано

Kernel Status -- Tainted:            IOE  X   
  
module=dcdbas             license=GPL               supported=external       
module=lpfc               license=GPL v2            supported=external       

модифицировано драйвером из данного RPM

SIGNATURE         VENDOR                                PACKAGE
(none)        Broadcom Inc. or its subsidiaries       elx-lpfc-kmp-default-14.0.639.23_k5.14.21_150400.24.46-1

драйвер с внешней поддержкой от производителя 

filename:       /lib/modules/5.14.21-150400.24.46-default/updates/lpfc.ko
supported:      external
version:        0:14.0.639.23
author:         Broadcom
description:    Emulex LightPulse Fibre Channel SCSI driver 14.0.639.23

необходимо обратится к производителю внешнего устройства для, получения корректного драйвера
