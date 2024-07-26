# TTS to Microphone
TTS to Microphone(TTStM) - это Text-to-Speech программа, которая озвучивает текст через микрофон, используя [Google TTS](https://pypi.org/project/gTTS/) и [VirtualCable](https://vb-audio.com/Cable/)

Основана на: [Python](https://www.python.org/), [Flet](https://flet.dev/) и [telebot](https://pypi.org/project/pyTelegramBotAPI/)

# Download guide
Заходите в [последний релиз](https://github.com/kamigearx12/TTS-to-Microphone/releases/tag/release)

![Pasted image 20240725174442](https://github.com/user-attachments/assets/43be660e-c419-4878-9ee2-dd442ffbd19e)

Листаете ниже и скачиваете архив с программкой

![Pasted image 20240725174909](https://github.com/user-attachments/assets/f8bbde11-3242-4b87-bad4-e5c06d300353)

Создаёте где-либо папку и перекидываете содержимое архива в созданную вами папку

![Pasted image 20240725175241](https://github.com/user-attachments/assets/475f606e-a7b6-4b2a-bdef-79086d44496c)

Запускаете ttstm.exe, устанавливаете драйвера и пользуетесь!

![Pasted image 20240725175350](https://github.com/user-attachments/assets/be91ee04-7b64-4215-8c57-59220b37c06c)

# Use guide
После того, как вы зашли в приложение, вы увидите довольно примитивный интерфейс.

![Pasted image 20240725183124](https://github.com/user-attachments/assets/d661f75b-23f9-4b2f-a639-04181ce695f6)

## Что здесь есть?
### Настройки
Первым делом, пользователю нужно зайти в настройки. Для чего?: Как минимум для того, что бы установить драйвера.

![Pasted image 20240725184022](https://github.com/user-attachments/assets/dcc6ec94-da63-46ad-9451-4682e499c28b)

#### Установка/Удаление драйверов
После установки нужно установить драйвера на виртуальный микрофон, через который будет озвучиваться текст.

**!!ВНИМАНИЕ!!**
**Для установки драйверов нужно запустить приложение от имени Администратора!**

Выбираете свою архитектуру здесь:

![Pasted image 20240725184250](https://github.com/user-attachments/assets/81e69b67-b302-4e5f-8084-fb62347ac9c1)

После выбора архитектуры открывается окошко с установкой драйвера

![Pasted image 20240725184336](https://github.com/user-attachments/assets/49cdd5bf-16fb-4247-9c06-ef8f7f74eb96)

На скриншоте видно кнопку **"Remove Driver"**, так как он у меня уже установлен. У вас будет кнопка **"Install Driver"**. Вы на неё нажимаете, разрешаете Windows добавить новое устройство, а после - перезагружаете систему.

**!!!Внимание!!!
После перезагрузки системы необходимо сменить динамики "CABLE Input" на свои динамики/наушники!**

![Pasted image 20240725184635](https://github.com/user-attachments/assets/f91d150b-e312-4c07-84d8-e8f5bc33864a)

После установки драйверов вы можете наконец приступать к использованию приложения. Таким же способом можно удалить драйвер, если он вам будет уже не нужен.

#### Выбор TTS языка
Для того, что бы пользоваться программой, вам необходимо выбрать язык, с акцентом и голосом которого будет говорить [Google TTS](https://pypi.org/project/gTTS/). По умолчанию выбран **Русский**.

Выбранный язык будет показан в заголовке приложения:

![Pasted image 20240725190510](https://github.com/user-attachments/assets/f40e5a44-7d7f-4f7f-a540-00ac04a96c64)

**!!!Внимание!!!
TTS язык - это НЕ язык интерфейса программы! Это язык, на котором текст будет озвучиваться! Для текста на Русском языке - Русский язык, для Украинского - Украинский, Английского - Английский. Каждый язык имеет свой собственный голос и акцент, который может не правильно работать на текста, написанным другим языком!**

#### Тёмная/Светлая тема
Кнопка **"Toggle Dark Mode"** переключает Тёмную и Светлую тему.

![Pasted image 20240725190002](https://github.com/user-attachments/assets/90ceca23-9e40-4c19-94b3-6487857d845e)


При первом заходе, по умолчанию, стоит Светлая тема. Тема сохраняется в файле theme, в папке с приложением, который создастся после первого захода в приложение.

![Pasted image 20240725190152](https://github.com/user-attachments/assets/61fc0b0a-2677-46e0-bbd1-905b50384449)\
![Pasted image 20240725190246](https://github.com/user-attachments/assets/2b5ce428-4379-40a4-a5a9-53aa981983ae)

#### Сохранение  **токена/API ключа**  от телеграмм бота
После нажатия на кнопку, введённый в поле **токен** будет сохранён в файле **"token"**, который будет создан в папке с приложением, после **первого захода/нажатия на кнопку**

![Pasted image 20240725191313](https://github.com/user-attachments/assets/6bfb5ebd-e24f-4b4e-9675-0206eec71d56)
![Pasted image 20240725191317](https://github.com/user-attachments/assets/bbd5a335-b079-4fea-a1f0-916e8a6c660b)

### Поле ввода и сообщения
В самом низу окошка мы видим текстовое поле, куда вводиться текст. После нажатия на **Enter**, или **кнопки отправки**, текст начнёт озвучиваться.

![Pasted image 20240725192127](https://github.com/user-attachments/assets/65e14d4b-83f8-4b7c-9724-bf17b31ad729)

Во время озвучки ваше сообщение будет выглядеть тёмным, а по окончанию озвучки - станет светлым. *(В чёрной теме наоборот: Во время озвучки сообщение светлое, а по окончанию - тёмное)*

![Pasted image 20240725192654](https://github.com/user-attachments/assets/26ccf4d6-0a25-4c9e-9973-fac4a6421444)
![Pasted image 20240725192822](https://github.com/user-attachments/assets/84b299e3-9250-4a4c-aec1-027346296622)

Во время озвучки текста поле ввода, а так же кнопка, недоступны. Это сделано для того, что бы не сломать программу.

### Личный TTSTM бот в Telegram
В программе доступна функция, которая позволяет запускать своего бота в телеграмм, который будет озвучивать введённый вами текст.

#### Для чего это нужно?
Благодаря этому вы можете отойти от своего рабочего места, взять телефон, и писать через него боту, который будет озвучивать текст на вашей рабочей машине.

#### Как создать бота и привязать его?
Для начала нам нужно создать бота через [BotFather](https://t.me/BotFather) в Telegram, после чего - скопировать **токен**.

![Pasted image 20240725194439](https://github.com/user-attachments/assets/d1938029-240f-4075-bcdd-98c381d6e3b0)

После этого заходим в приложение, и нажимаем на иконку глаза:

![Pasted image 20240725195721](https://github.com/user-attachments/assets/76db52c1-d21b-47fa-a9ae-e69be0b42e74)

После, вводим токен в поле ввода:

![Pasted image 20240725195932](https://github.com/user-attachments/assets/57b89a1d-9732-4252-83b1-d07f4bea453a)
![Pasted image 20240725200029](https://github.com/user-attachments/assets/30be6bf9-64ad-4dab-a46d-06f375efaf3d)

После вставки токена, мы можем сохранить его в настройках, а после - запустить бота, нажав на облако:

![Pasted image 20240725200158](https://github.com/user-attachments/assets/0d40358a-4812-4ddd-9354-bcaa7ba328bd)

Нажав на это облако ещё раз, мы вырубим бота.

#### Как пользоваться ботом?
После запуска бота, мы пишем ему команду **/start или /help**

![Pasted image 20240725200657](https://github.com/user-attachments/assets/e88f8a76-340e-4e6b-a13b-a5598bdcf109)

- Командой **/lang** мы видим выбранный сейчас TTS язык.
- Командой **/ru, /uk и /en** мы меняем TTS язык *(по умолчанию стоит тот, что был в программе)*.

Далее просто пишем нужный текст, и он будет озвучен через микрофон.

![Pasted image 20240725201328](https://github.com/user-attachments/assets/0735ac93-c17d-4d00-a2e2-ef20fcb1c9d3)
