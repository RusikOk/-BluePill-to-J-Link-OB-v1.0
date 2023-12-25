# programmer-BluePill-to-J-Link-OB-v1.0
успешная попытка создать программатор J-Link OB v1.0 на чипе CS32F103C8T6

в общем валялось у меня пару лет макетка с кристалом CS32F103. использовать в своих разработках я бы такое не стал. а в качестве J-Link OB они зашли на ура.

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P01215-040605.jpg" alt="какашка"> 

<h2>REV 1.0</h2>

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%201.0/P01128-204354%20comment.jpg" alt="top"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%201.0/P01128-204404%20comment.jpg" alt="bottom"> 
<br>
выявленные недостатки:<br>
- очень бесит когда при обновлении прошивки она тупо слетает в следствии использования мной МК на 64кБ. в идеале нужно использовать МК на 128кБ флешки. хотя если не шляться по чужим компам и постоянно не обновлять библиотеки jLink то жить можно.<br>
- маленькая нагрузочная способность встроенного в BluePill LDO всего на 300мА, что не позволяет запитывать target током больше 250мА.<br>
- при подключении target на горячую проседает питание программатора и он отваливается. приходится перетыкать USB.<br>
<br>
ссылки:<br>
<a href="http://forum.easyelectronics.ru/viewtopic.php?p=649897#p649897">J-Link OB (On-Board)</a><br>

<h2>REV 1.1</h2>

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/3_schematic/%D0%BC%D0%BE%D1%80%D0%B3%D0%B0%D0%BB%D0%BA%D0%B0.jpg" alt="schematic">
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%201.0/P20428-160107%20moding.jpg" alt="bottom">
выявленные недостатки:<br>
- вход таймера нужно было подключать к SW_DIO чтобы при отключенном target светодиод не моргал.<br>

<h2>REV 2.0</h2>

особенностью второй версии программатора является возможность запитки целевой платы током до 1А благодаря применению понижающего DC-DC преобразователя напряжения.<br>
<br>
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P01215-040734%20comment.jpg" alt="top"> 
1) проверить все номиналы резисторов на DC-DC, китайцы могут вариировать номиналы<br>
2) не помню перерезана перемычка ADJ с обратной стороны DC-DC или нет. проверить<br>
3) на синий светодиод SW_CLK желательно поставить транзистор в ключевом режиме дабы по минимуму нагружать вывод МК<br>
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P01215-040827%20comment.jpg" alt="bottom"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P10424-114441.jpg" alt="top"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P10424-114515.jpg" alt="bottom"> 
<br>
выявленные недостатки:<br>
- очень бесит когда при обновлении прошивки она тупо слетает в следствии использования мной МК на 64кБ. в идеале нужно использовать МК на 128кБ флешки. хотя если не шляться по чужим компам и постоянно не обновлять библиотеки jLink то жить можно.<br>
- оказалась неудачной компоновка светодиодов зеленый (USB) и синий (SW_CLK) сливаются в следствии чего через корпус не видно происходит обмен с target или нет. зеленый светодиод нужно оставить на месте возле разъема USB а синий перенести на противоположную сторону платы. возможно использовать DIP корпус диаметром 3мм.<br>
- на больших скоростях обмена синий светодиод (SW_CLK) очень слабо виден. поэтому как вариант поставить одновибратор на LMC555 таймере для выравнивания длительности свечения светодиода.<br>
<br>
ссылки:<br>
<a href="https://mysensors-rus.github.io/Blue-pill-to-JLink/">Делаем из BluePill пограмматор/отладчик JLink OB-STM32F103</a><br>
<a href="http://forum.easyelectronics.ru/viewtopic.php?p=650368#p650368">J-Link OB (On-Board)</a><br>
<a href="http://easyelectronics.ru/malenkaya-xitrost.html">Маленькая хитрость</a><br>
<a href="http://we.easyelectronics.ru/STM32/cs32f103c8t6-gd32f103cbt6-i-drugie-kitayskie-klony-stm32f103c8t6-i-stm32f030c8t6.html">китайские клоны STM32</a><br>

<h2>BOX</h2>

<a href="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/6_3D%20%D0%BF%D0%B5%D1%87%D0%B0%D1%82%D1%8C/for%20Dobot%20Mooz%202%20-%20PLA.curaprofile">настройки слайсера Ultimaker Cura для генерации G-кода для 3D принтера Dobot Mooz 2</a>

<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/5_SolidWorks2020/untitled.46.png"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/5_SolidWorks2020/untitled.47_2.png"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P10424-124740.jpg" alt="box"> 
<img src="https://github.com/RusikOk/-BluePill-to-J-Link-OB-v1.0/blob/main/7_photo/rev%202.0/P10424-124813.jpg" alt="box">