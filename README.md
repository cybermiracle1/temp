#### предварительный анализ логов выявил ошибки 

`messages_localwarn.txt:2023-03-05T15:43:43.903032+03:00 xxidb3 kernel: [10795.014472][T31147] nvme nvme1: NVME-FC{1}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:43.903047+03:00 xxidb3 kernel: [10795.014485][T31147] nvme nvme5: NVME-FC{5}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:43.903054+03:00 xxidb3 kernel: [10795.014495][T31147] nvme nvme0: NVME-FC{0}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:43.903055+03:00 xxidb3 kernel: [10795.014504][T31147] nvme nvme3: NVME-FC{3}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:44.783032+03:00 xxidb3 kernel: [10795.893773][T31147] nvme nvme6: NVME-FC{6}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:44.783042+03:00 xxidb3 kernel: [10795.893784][T31147] nvme nvme2: NVME-FC{2}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:44.783045+03:00 xxidb3 kernel: [10795.893793][T31147] nvme nvme7: NVME-FC{7}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T15:43:44.783047+03:00 xxidb3 kernel: [10795.893801][T31147] nvme nvme4: NVME-FC{4}: controller connectivity lost.`

`messages_localwarn.txt:2023-03-05T16:00:55.904017+03:00 xxidb3 kernel: [  202.345723][  T552] nvme nvme3: NVME-FC{3}: transport association event: transport detected io error`

`messages_localwarn.txt:2023-03-05T16:00:55.904020+03:00 xxidb3 kernel: [  202.345727][  T552] nvme nvme3: NVME-FC{3}: resetting controller`

`messages_localwarn.txt:2023-03-05T16:00:55.944012+03:00 xxidb3 kernel: [  202.385617][  T552] nvme nvme3: NVME-FC{3}: error_recovery: Couldn't change state to CONNECTING`

`messages_localwarn.txt:2023-03-05T16:08:24.416021+03:00 xxidb3 kernel: [  650.858079][  T522] nvme nvme1: NVME-FC{1}: transport association event: transport detected io error`

`messages_localwarn.txt:2023-03-05T16:08:24.416030+03:00 xxidb3 kernel: [  650.858082][  T522] nvme nvme1: NVME-FC{1}: resetting controller`

`messages_localwarn.txt:2023-03-05T16:08:24.456010+03:00 xxidb3 kernel: [  650.894379][  T522] nvme nvme1: NVME-FC{1}: error_recovery: Couldn't change state to CONNECTING`



`hardware.txt:<6>[  778.682900][ T7739] nvme nvme5: NVME-FC{5}: create association : host wwpn 0x100008f1eabf3dbe  rport wwpn 0x20002811eceddcf7: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<3>[  778.683045][ T7739] nvme nvme5: Connect command failed: host path error`

`hardware.txt:<6>[  801.279455][ T1178] nvme nvme0: NVME-FC{0}: controller connectivity lost. Awaiting Reconnect`

`hardware.txt:<6>[  801.294714][ T6455] nvme nvme0: Removing ctrl: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  802.415751][ T1111] nvme nvme4: NVME-FC{4}: controller connectivity lost. Awaiting Reconnect`

`hardware.txt:<6>[  802.422166][  T524] nvme nvme0: NVME-FC{0}: create association : host wwpn 0x100008f1eabf3dbe  rport wwpn 0x20102811eceddcf7: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  802.422709][   C13] nvme nvme0: NVME-FC{0}: io failed due to bad NVMe_ERSP: iu len 8, xfr len 4096 vs 0, status code 1, cmdid 8210 vs 8210`

`hardware.txt:<4>[  802.422715][  T524] nvme nvme0: queue_size 128 > ctrl maxcmd 0, reducing to maxcmd`

`hardware.txt:<6>[  802.422723][  T524] nvme nvme0: NVME-FC{0}: controller connect complete`

`hardware.txt:<6>[  802.422728][ T7784] nvme nvme0: NVME-FC{0}: new ctrl: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  802.454700][ T6463] nvme nvme4: Removing ctrl: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  803.542381][ T7049] nvme nvme4: NVME-FC{4}: create association : host wwpn 0x100008f1eabf3dbd  rport wwpn 0x20112811eceddcf7: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  803.542893][    C1] nvme nvme4: NVME-FC{4}: io failed due to bad NVMe_ERSP: iu len 8, xfr len 4096 vs 0, status code 1, cmdid 8202 vs 8202`

`hardware.txt:<4>[  803.542900][ T7049] nvme nvme4: queue_size 128 > ctrl maxcmd 0, reducing to maxcmd`

`hardware.txt:<4>[  803.542903][  T524] nvme nvme4: NVME-FC{4}: transport association event: transport detected io error`

`hardware.txt:<4>[  803.542906][  T524] nvme nvme4: NVME-FC{4}: resetting controller`

`hardware.txt:<6>[  803.542908][ T7049] nvme nvme4: NVME-FC{4}: controller connect complete`

`hardware.txt:<6>[  803.542914][ T7791] nvme nvme4: NVME-FC{4}: new ctrl: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<6>[  803.543121][ T7791] nvme nvme4: Removing ctrl: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<3>[  803.586639][  T524] nvme nvme4: NVME-FC{4}: error_recovery: Couldn't change state to CONNECTING`

`hardware.txt:<6>[  803.586650][ T7049] nvme nvme4: NVME-FC{4}: create association : host wwpn 0x100008f1eabf3dbd  rport wwpn 0x20112811eceddcf7: NQN "nqn.2014-08.org.nvmexpress.discovery"`

`hardware.txt:<3>[  803.586768][ T7049] nvme nvme4: Connect command failed: host path error`

#### судя по всему NVME диски подключены через внешнее устройство накопитель и проблема в драйвере контроллера 

#==[ Configuration File ]===========================#

#/proc/sys/kernel/tainted
79872


Kernel Status -- Tainted:            IOE  X   

  TAINT: (I) Working around severe firmware bug
  
  TAINT: (O) Out-of-tree module has been loaded
  
  TAINT: (E) Unsigned module has been loaded
  
  TAINT: (X) Modules with external support loaded

module=dcdbas             license=GPL               supported=external      

module=lpfc               license=GPL v2            supported=external       

#==[ Command ]======================================#

#/bin/dmesg -T | grep taint

[Sun Mar  5 17:32:35 2023] lpfc: loading out-of-tree module taints kernel.

[Sun Mar  5 17:32:35 2023] lpfc: loading out-of-tree module taints kernel.

[Sun Mar  5 17:32:35 2023] lpfc: module verification failed: signature and/or required key missing - tainting kernel

[Sun Mar  5 17:32:35 2023] lpfc: externally supported module, setting X kernel taint flag.

[Sun Mar  5 17:32:40 2023] dcdbas: externally supported module, setting X kernel taint flag.


####  драйвер контроллера внешнего накопителя

`SIGNATURE`         `VENDOR`                               `PACKAGE`

`(none)`        `Broadcom Inc. or its subsidiaries`       `elx-lpfc-kmp-default-14.0.639.23_k5.14.21_150400.24.46-1`

#### драйвер с внешней поддержкой от производителя 

#==[ Command ]======================================#

#/sbin/modinfo lpfc

filename:       /lib/modules/5.14.21-150400.24.46-default/updates/lpfc.ko

`supported:      external`

version:        0:14.0.639.23

author:         Broadcom

description:    Emulex LightPulse Fibre Channel SCSI driver 14.0.639.23

#### необходимо обратится к производителю внешнего устройства для получения корректного драйвера
