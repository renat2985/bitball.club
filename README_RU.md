# Умный Fight Ball (Box Ball) на базе ESP8266

<a href="https://www.youtube.com/watch?v=Eb2ycZCe_rk&list=PL6NJTNxbvy-JwHCaki6eOuAYkdLQA4lqW"><img src="https://github.com/renat2985/bitball.club/blob/main/doc/bitball3.png"></a>

Это усовершенствованная версия классической игры с мячом на резинке (Box Ball), которая направлена на развитие координации, скорости реакции и ловкости. В отличие от стандартного мячика, наша разработка оснащена умной электроникой на базе микроконтроллера ESP8266 (NodeMCU), что позволяет вести учет количества ударов, измерять силу удара и соревноваться по интернету через сайт [bitball.club](http://bitball.club) с другими пользователями, у которых есть такие же устройства. Также можно отслеживать прогресс игрока в реальном времени.

Вы можете собрать устройство самостоятельно или попросить это сделать для вас. Для заказа готового устройства свяжитесь через [Telegram](https://t.me/ESPiotDevice), [WhatsApp](https://chat.whatsapp.com/LZ9tSHqVLDEFJ41Vte2PZ1), [Skype](https://skype:renat2985?chat), [Discord](https://discord.gg/3986vwEdf5).

## Основные функции:
- **Отслеживание ударов**: Устройство использует встроенные датчики, чтобы точно фиксировать каждый удар по мячу.
- **Подсчет силы удара**: Устройство анализирует данные с датчиков, чтобы измерять силу удара, что добавляет элемент соревнования.
- **Подключение к Wi-Fi**: Устройство может подключаться к сети Wi-Fi, что позволяет сохранять результаты тренировок в облаке и участвовать в онлайн-турнирах.
- **Гибкая настройка тренировок**: Возможность установки времени тренировок и других параметров для адаптации устройства под личные цели пользователя.
- **Обратная связь**: Система звукового или светового оповещения помогает вовремя завершить тренировку или мотивировать пользователя на улучшение результатов.
- **Онлайн-соревнования**: Возможность соревноваться в реальном времени с другими пользователями через сайт [bitball.club](http://bitball.club), сравнивать результаты и повышать уровень своих тренировок.

## Преимущества:
- **Интерактивность**: Тренировки становятся более захватывающими и интерактивными благодаря системе автоматического подсчета, измерению силы удара и мгновенной обратной связи.
- **Соревнования в реальном времени**: Пользователи могут соревноваться друг с другом, создавая глобальную сеть игроков, что делает процесс тренировок ещё более увлекательным.

Наш умный Box Ball – это не просто мяч на резинке, это высокотехнологичное устройство для тренировок, которое позволяет вам ставить цели, отслеживать прогресс, измерять силу ударов и достигать новых высот в развитии координации и реакции.

## Инструкция

### Включение устройства:
- **Первый сигнал**: Устройство успешно включено.
- **Второй сигнал (индикация заряда)**:
  - Высокая тональность — заряд 100%.
  - Средняя тональность — заряд 50%.
  - Низкая тональность — заряд 25%. В этом режиме звук отключается для экономии энергии.
- **Третий сигнал (через 4-15 секунд — режим работы)**:
  - Высокая тональность — устройство подключено к роутеру.
  - Низкая тональность — подключение к роутеру не удалось. Устройство создало WiFi-точку "BitBall.club".

- **Авто засыпание**: Если в течение 5 минут игра не была запущена, устройство переходит в режим сна. Сигнал о переходе в режим сна: звук высокой тональности, который плавно понижается до низкой тональности.

### Как начать игру с BitBall
1. Включите устройство BitBall.
2. Подключитесь к Wi-Fi:
   - Выберите сеть BitBall.club.

      <img src="https://github.com/renat2985/bitball.club/blob/main/doc/WiFi.png" width="200px">

3. Доступ к игре через браузер:
   - Откройте браузер и введите адрес: `http://192.168.4.1`.

      <img src="https://github.com/renat2985/bitball.club/blob/main/doc/AP.gif" width="300px">


#### **Совет**: Если вы подключите BitBall к своему роутеру, вам не придется каждый раз подключаться к Wi-Fi BitBall.club. Просто перейдите на [www.bitball.club](http://www.bitball.club), и вы сразу окажетесь в игре. + вы сможете сохранять результаты ствоих тренеровок, соревноваться с другими людьми в онлайн и много других плюшек.

# HTTP и безопасность

Наше устройство использует WebSocket без SSL, что не позволяет ему работать через HTTPS. Поэтому мы оставили [www.bitball.club](http://www.bitball.club) доступным только по протоколу HTTP.

Однако это никак не влияет на вашу безопасность, так как сайт не требует ввода паролей или другой конфиденциальной информации.

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/security.gif" width="500px">

## Схема подключения

На плате NodeMCU кнопка Flash выполняет те же функции, что и внешняя кнопка, подключенная к D3. При необходимости вы можете использовать её вместо внешней кнопки.

### Простая

| Pin            | GPIO  | Назначение    |
|----------------|-------|---------------|
| D1             | GPIO5 | SCK (HX711)   |
| D2             | GPIO4 | DT (HX711)    |
| D3             | GPIO0 | Button        |

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicEasy.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemosEasy.png" width="300px">

### Продвинутая

| Pin            | GPIO  | Назначение    |
|----------------|-------|---------------|
| D5             | GPIO14| Buzzer        |
| D6             | GPIO12| Led           |
| D7             | GPIO13| Vibro Motor   |

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematic.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemos.png" width="300px">


## STL (stl папка)
Эта подложка необходима для корректной работы датчика веса; без неё возможны ложные срабатывания. Важно, чтобы внутренняя часть весов не соприкасалась с лбом или другими поверхностями.

<img src="https://github.com/renat2985/bitball.club/blob/main/stl/sensorBoxFinal.png" height="200px"> <img src="https://github.com/renat2985/bitball.club/blob/main/stl/box.png" height="200px"> <img src="https://github.com/renat2985/bitball.club/blob/main/stl/cover.png" height="200px"> 

## Компоненты

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/canva.jpg" height="100px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9764.JPG" height="100px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9752.JPG" height="100px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9749.JPG" height="100px">

## From AliExpress.com

[Tennis Training Ball with Elastic String](https://www.aliexpress.com/item/1005008118081299.html) (Вам нужен именно теннисный мяч с резинкой. Мячи от Fight Ball не подходят, так как они слишком лёгкие)  

[Flashlight Headband Head Strap 18650](https://www.aliexpress.com/item/1005006141023865.html) (Вам нужна резинка для головы с креплением для powerbank)

[Weight Sensors + HX711](https://www.aliexpress.com/item/1005006293517345.html)

[Power Bank (for 18650 Battery)](https://www.aliexpress.com/item/1005002367815544.html)

[Wemos MINI](https://www.aliexpress.com/item/1005001621784437.html) (потходит для STL корпуса) или [NodeMCU ESP8266](https://www.aliexpress.com/item/1005004893349830.html)

Опционально для более сложной модели:  

[Head Straps Headband](https://www.aliexpress.com/item/1005005898038310.html)

[Nylon Elastic Band](https://www.aliexpress.com/item/1005002060362335.html) (Ширина 2.5cm)

[Elastic Band Round](https://www.aliexpress.com/item/4000977316378.html)

[ULN2003A](https://www.aliexpress.com/item/32556525207.html)

[USB Type A Connector Male](https://www.aliexpress.com/item/32924785370.html)

[Push Button Switch](https://www.aliexpress.com/item/1005004159746274.html)

[Passive Buzzer Module for Arduino](https://www.aliexpress.com/item/1005005528181661.html) или [Passive Buzzer 5v](https://www.aliexpress.com/item/1005006260328559.html) (Для ULN2003A)

---

## 🚀 Веб-установщик (рекомендуется)

### Перейдите на веб-установщик и следуйте инструкциям.

## [https://renat2985.github.io/bitball.club/](https://renat2985.github.io/bitball.club/)

---

## :battery: Donation

If you like this project, you can buy me a cup of coffee :coffee:

<img src="https://github.com/renat2985/renat2985/raw/main/donate/donate.png" width="100%">

- PayPal [https://www.paypal.me/RKevrels](https://www.paypal.me/RKevrels/5)