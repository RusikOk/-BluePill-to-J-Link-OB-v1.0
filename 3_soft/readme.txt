﻿последовательность прошивки самого программатора compiled Apr 8 2020 10:10:28 	(НЕ АКТУАЛЬНО)

1) зашить прошивку 1_2019_jlink-obSTM32F103.bin
2) запустить утилиту JLink.exe из старой версии драйверов c:\Program Files (x86)\SEGGER\JLink_V500\
3) установить новый серийный номер коммандой "exec SetSN=20201111"
4) зашить прошивку 2_JLink_OB_STM32F103_V1_compiled_Apr_8_2020.bin

(с) RusikOk 2020-11-29

последовательность прошивки новой версии программатора compiled Feb 2 2021 16:45:54

1) зашить прошивку 3_JLink_OB_STM32F103_V1_compiled Feb 2 2021.bin
2) запустить утилиту JLink.exe из старой версии драйверов c:\Program Files (x86)\SEGGER\JLink_V500\
3) установить новый серийный номер коммандой "exec SetSN=20211111"

(с) RusikOk 2021-04-21

последовательность создания новой версии прошивки программатора для МК CS32F103

1) зашить прошивку 4_JLOB103V1_bootloader.bin
2) подключаем J-Link к компьютеру по USB и запускаем J-Link Commander, а он уже установит актуальную версию прошивки
3) запустить утилиту JLink.exe из старой версии драйверов c:\Program Files (x86)\SEGGER\JLink_V500\
4) установить новый серийный номер коммандой "exec SetSN=20211111"

(с) RusikOk 2021-04-21