# -BluePill-to-J-Link-OB-v1.0
успешная попытка создать программатор J-Link OB v1.0 на чипе CS32F103C8T6

в общем валялось у меня пару плат с кристалом CS32F103. использовать в своих разработках я бы такое не стал. а в качестве J-Link OB они зашли на ура.

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P01215-040605.jpg" alt="какашка"> 

<h2>REV 1.0</h2>

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%201.0/P01128-204354%20comment.jpg" alt="top"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%201.0/P01128-204404%20comment.jpg" alt="bottom"> 
<br>
ссылки:<br>
<a href="http://forum.easyelectronics.ru/viewtopic.php?p=649897#p649897">J-Link OB (On-Board)</a><br>

<h2>REV 2.0</h2>

особенностью второй версии программатора является возможность запитки целевой платы током до 1А благодаря применению понижающего DC/DC преобразователя напряжения.
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P01215-040734%20comment.jpg" alt="top"> 
1) проверить все номиналы резисторов на DC-DC, китайцы могут вариировать номиналы<br>
2) не помню перерезана перемычка ADJ с обратной стороны DC-DC или нет. проверить<br>
3) на светодиод CLK желательно поставить транзистор в ключевом режиме дабы по минимуму нагружать вывод МК<br>
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P01215-040827%20comment.jpg" alt="bottom"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P10424-114441.jpg" alt="top"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P10424-114515.jpg" alt="bottom"> 
<br>
ссылки:<br>
<a href="https://mysensors-rus.github.io/Blue-pill-to-JLink/">Делаем из BluePill пограмматор/отладчик JLink OB-STM32F103</a><br>
<a href="http://forum.easyelectronics.ru/viewtopic.php?p=650368#p650368">J-Link OB (On-Board)</a><br>
<a href="http://easyelectronics.ru/malenkaya-xitrost.html">Маленькая хитрость</a><br>

<h2>BOX</h2>

<a href="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/5_3D%20%D0%BF%D0%B5%D1%87%D0%B0%D1%82%D1%8C/for%20Dobot%20Mooz%202%20-%20PLA.curaprofile">настройки слайсера Ultimaker Cura для генерации G-кода для 3D принтера Dobot Mooz 2</a>

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/4_SolidWorks2020/untitled.46.png"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/4_SolidWorks2020/untitled.47_2.png"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P10424-124740.jpg" alt="box"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_%D1%84%D0%BE%D1%82%D0%BE/rev%202.0/P10424-124813.jpg" alt="box">