
### Светодиодная панель
Плата позволяет работать со светодиодной панелью до 255 точек по любой из осей. По умолчанию настроена работа с матрицей 128 х 16, формат заполнения пикселей - 'вертикальный зигзаг', формат цвета -  `GreenRedBlue`. Файлы анимаций хранятся на SD-карте в формате PXL (редактор http://pxledit.starpixel.org/). 
Каждая анимация является слоем. Слои заполняются с id = 0 и до id = 7 с учетом прозрачности. Все не прозрачные пиксели слоя id = 1 изменят значения пикселей слоя с id = 0. Все файлы должны находится в папке `led_pxl_r` SD-карты. Для повышения производительности настоятельно рекомендуется рисовать все изображения с прозрачным фоном, если это позволяет дизайн.
Описание слоёв:
 * `layer0.pxl` - Фоновый слой;
 * `layer1.pxl` - Фоновая анимация;
 * `layer2.pxl` - Габаритные огни;
 * `layer3.pxl` - Задний ход;
 * `layer4.pxl` - Стоп-сигналы;
 * `layer5.pxl` - Повороты влево;
 * `layer6.pxl` - Повороты вправо;
 * `layer7.pxl` - Аварийный сигнал;
 
 
 ### Силовые выходы
На плате находится 6 силовых выходов до 10А каждый, до 25А в сумме, для подключения осветителей. Выходы имеют контроль тока и электронную защиту от короткого замыкания. Управление происходит по плюсу (размыкается плюсовой контакт, минус общий и не размыкается). Описание выходов:
* `CH1` - Доп. освещение;
* `CH2` - Габаритные огни;
* `CH3` - Задних ход;
* `CH4` - Стоп-сигнал;
* `CH5` - Повороты влево;
* `CH6` - Повороты вправо;

