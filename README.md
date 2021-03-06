### Альтернативная схемотехника автономного устройства для передачи показаний воды по Wi-Fi - Ватериус.

<img src="https://github.com/badenbaden/Waterius-Attiny84-ESP12F/blob/master/Visualization/abb-ap9-3.jpg" data-canonical-src="https://github.com/badenbaden/Waterius-Attiny84-ESP12F/blob/master/Visualization/abb-ap9-3.jpg" width="400"/>
<img src="https://github.com/badenbaden/Waterius-Attiny84-ESP12F/blob/master/Foto/%D0%92%20%D0%BA%D0%BE%D1%80%D0%BF%D1%83%D1%81%D0%B5%202.jpg" width="400"/>
<img src="https://github.com/badenbaden/Waterius-Attiny84-ESP12F/blob/master/Foto/%D0%92%20%D0%BA%D0%BE%D1%80%D0%BF%D1%83%D1%81%D0%B5%203.jpg" width="400"/>


[Оригинальная версия, взятая за основу](https://github.com/dontsovcmc/waterius/)

[Обсуждение данной версии, испытания, симуляции и т.д.](https://github.com/dontsovcmc/waterius/issues/128)

### Текущий статус:
- Бета версия.
- Устройство [изготовлено](https://github.com/badenbaden/Waterius-Attiny84-ESP12F/tree/master/Foto), пишется прошивка.
- На текущий момент работают 4 счетчика, 2 датчика протечки. Отображение в облаке Ватериус только 2х счетчиков, датчики протечки также не отображаются.
- Тестовые прошивки: [Вторая Бета](https://github.com/badenbaden/Waterius-Attiny84-ESP12F/tree/master/Firmware/SecondBeta)
[Первая Бета](https://github.com/badenbaden/Waterius-Attiny84-ESP12F/tree/master/Firmware/FirstBeta)
=======
- На текущий момент работают 4 счетчика, 2 датчика протечки, отправляет оповещение при протечке (пока только одного канала). Отображение в облаке Ватериус только 2х счетчиков.
- Тестовые прошивки [тут](https://github.com/badenbaden/Waterius-Attiny84-ESP12F/tree/master/Firmware/FirstBeta).

### Планируемые возможности:
- 4 счётчика воды (вам не нужно знать, какого типа выход: "сухой контакт" или "НАМУР")
- передача по Wi-Fi раз в сутки
- питание 3 АА батарейки (~4 года работы)
- не нужно знать, сколько литров на импульс (Ватериус сам определит 1 или 10л/имп)
- корпус с защитой от пыли и воды (IP65) 
- контроль напряжения батареи
- 2 независимых канала для датчиков протечки (для лучшего понимания зоны возможной протечки)
- индикация протечки светодиодом, передача тревожного сообщения на сайт, mqtt
- отдельный вывод сигнала протечки (для передачи на внешние исполнители или информеры)
- вывод под датчик температуры (подключен к есп8266, т.е. контроль возможен не чаще включения WiFi)
- полное отключение есп8266 от питания, для продление жизни батарей
- использование есп8266 версии 12E, 12F или 12S
- выведены на плате GPIO9, GPIO10, GPIO12, GPIO14
- отдельные порты для прошивки и мониторинга attiny и esp
- может еще что забыл))

### Прошивка:
С прошивкой обещал помочь автор оригинального ватериуса - @dontsovcmc
