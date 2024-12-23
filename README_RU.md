# Умный Fight Ball (Box Ball) на базе ESP8266

<a href="https://www.youtube.com/watch?v=ykzgbnOf2mE&list=PL6NJTNxbvy-JwHCaki6eOuAYkdLQA4lqW&pp=gAQB"><img src="https://github.com/renat2985/bitball.club/blob/main/doc/bitball3.png"></a>

Это усовершенствованная версия классической игры с мячом на резинке (Box Ball), которая направлена на развитие координации, скорости реакции и ловкости. В отличие от стандартного мячика, наша разработка оснащена умной электроникой на базе микроконтроллера ESP8266 (NodeMCU), что позволяет вести учет количества ударов, измерять силу удара и соревноваться по интернету через сайт [bitball.club](https://bitball.club) с другими пользователями, у которых есть такие же устройства. Также можно отслеживать прогресс игрока в реальном времени.

Вы можете собрать устройство самостоятельно или попросить это сделать для вас. Для заказа готового устройства свяжитесь через [Telegram](https://t.me/ESPiotDevice), [Skype](https://skype:renat2985?chat), [Discord](https://discord.com/invite/zaGaDuGe).

## Основные функции:
- **Отслеживание ударов**: Устройство использует встроенные датчики, чтобы точно фиксировать каждый удар по мячу.
- **Подсчет силы удара**: Устройство анализирует данные с датчиков, чтобы измерять силу удара, что добавляет элемент соревнования.
- **Подключение к Wi-Fi**: Устройство может подключаться к сети Wi-Fi, что позволяет сохранять результаты тренировок в облаке и участвовать в онлайн-турнирах.
- **Гибкая настройка тренировок**: Возможность установки времени тренировок и других параметров для адаптации устройства под личные цели пользователя.
- **Обратная связь**: Система звукового или светового оповещения помогает вовремя завершить тренировку или мотивировать пользователя на улучшение результатов.
- **Онлайн-соревнования**: Возможность соревноваться в реальном времени с другими пользователями через сайт [bitball.club](https://bitball.club), сравнивать результаты и повышать уровень своих тренировок.

## Преимущества:
- **Интерактивность**: Тренировки становятся более захватывающими и интерактивными благодаря системе автоматического подсчета, измерению силы удара и мгновенной обратной связи.
- **Соревнования в реальном времени**: Пользователи могут соревноваться друг с другом, создавая глобальную сеть игроков, что делает процесс тренировок ещё более увлекательным.

Наш умный Box Ball – это не просто мяч на резинке, это высокотехнологичное устройство для тренировок, которое позволяет вам ставить цели, отслеживать прогресс, измерять силу ударов и достигать новых высот в развитии координации и реакции.

## Контакты

#### Вы можете собрать устройство самостоятельно или попросить сделать это за вас. Чтобы заказать готовое устройство, свяжитесь со мной через [Telegram](https://t.me/ESPiotDevice), [Skype](https://skype:renat2985?chat), или [Discord](https://discord.com/invite/zaGaDuGe).


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


#### **Совет**: Если вы подключите BitBall к своему роутеру, вам не придется каждый раз подключаться к Wi-Fi BitBall.club. Просто перейдите на [www.bitball.club](https://www.bitball.club), и вы сразу окажетесь в игре. + вы сможете сохранять результаты ствоих тренерово, соревноваться с другими людьми в онлайн и много других плюшек.


## Схема подключения
### Простая
NodeMCU ESP8266, Wemos ESP8266

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicEasy.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemosEasy.png" width="300px">

### Продвинутая
NodeMCU ESP8266, Wemos ESP8266

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematic.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemos.png" width="300px">


## STL (3d print папка)
Эта подложка необходима для корректной работы датчика веса; без неё возможны ложные срабатывания. Важно, чтобы внутренняя часть весов не соприкасалась с лбом или другими поверхностями.

<img src="https://github.com/renat2985/bitball.club/blob/main/3d%20print/sensorBox.png" height="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/3d%20print/sensorBoxAUX.png" height="300px"> 

## Компоненты

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/components/canva.png" height="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9764.png" width="400px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9752.png" width="400px">

## From AliExpress.com

<sup>https://www.aliexpress.com/item/1005004893349830.html - NodeMCU ESP8266</sup>

<sup>https://www.aliexpress.com/item/1005006293517345.html - Weight Sensors + HX711</sup>

<sup>https://www.aliexpress.com/item/32556525207.html - ULN2003A</sup>

<sup>https://www.aliexpress.com/item/1005002060362335.html - Nylon Elastic Band</sup>

<sup>https://www.aliexpress.com/item/4000977316378.html - Elastic Band Round</sup>

<sup>https://www.aliexpress.com/item/1005002367815544.html - Power Bank (for 18650 Battery) </sup>

<sup>https://www.aliexpress.com/item/1005005898038310.html - Head Straps Headband</sup>


## 🚀 Web installer (recommended)

### Go to the web installer and follow instructions.

## [https://renat2985.github.io/bitball.club/](https://renat2985.github.io/bitball.club/)


## :battery: Donation

If you like this project, you can buy me a cup of coffee :coffee:

<img src="https://github.com/renat2985/renat2985/raw/main/donate/donate.png" width="100%">

- PayPal [https://www.paypal.me/RKevrels](https://www.paypal.me/RKevrels/5)