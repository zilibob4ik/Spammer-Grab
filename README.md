# Spammer-Grab
A brand new, awakened version of the old Spammer-Grab. Spammer-Grab is a script used to spam Grab Activation Code or GAC to a phone number.
## What's new?
Nothing really new here. I rewritten the whole script and refactored them. The code is pretty neat compared to the previous one (no more bytecodes). Also, I managed to leave Python 2, now the code only supports Python 3.7 and later.
### Piece of history
This project was actually here since the June 2017. This is one of my first project in GitHub. Back then, it works really well. Few months later, it turned out to be not working (because of an unknown thing :/). Then, I deleted this repository at the beginning of this year. Again, few months later, I heard that someone has been making a patch for the issue (using someone's fork of the old version of this repo). It is so complex (lots of forking made me confused) that I don't even know who made the patch. At the end of the day, here is the new Spammer-Grab for those who wants to use it :).
#### Why do I made this "new version"?
There are some people who contacts me, they said that they want a new working version of this project. That's why I made this, this is only for people who needs it.
## Installation
You need at least Python 3.7 to run this new Spammer-Grab. First of all, you need to clone this repository.
```
git clone https://github.com/p4kl0nc4t/Spammer-Grab
```
Install all the required modules using `pip`.
```
pip install -r REQUIREMENTS
```
## Usage
```
Usage: spammer.py [OPTIONS] PHONE_NUM

  This script will repeatedly send Grab Activation Code (GAC) to PHONE_NUM.
  PHONE_NUM must be a phone number in international format (example:
  6281323323232 with 62 prefix as the country code)

Options:
  -dl, --delay INTEGER      delay between each request wave
  -li, --limit INTEGER      amount of request to send
  -cc, --country_code TEXT  phone number country code
  --help                    Show this message and exit.
```
## License
This project is licensed with MIT License.
## Contribution
Feel free to contribute to this project. Any kind of contribution is really appreciated.

1. Телефон (Android)
2. Программа Termux (эмулятор линукс)
3. Интернет на телефоне ( Лучше WiFi )
И так приступим, первым делом берём в свою правую или левую мощную руку телефон, заходим в Google Play и забиваем в поиск "Termux ", качаем и устанавливаем.
Далее заходим в программу " Termux "
И пишем туда как пишу я, все слова с новой строчки. Да, всё вводим руками, не ленимся.
(если требует соглашение то вводим в строку "Y" без кавычек и жмем ввод)

Вводим каждую строку отдельно:
Clear
pkg update
pkg install git
pkg install python
pkg install python2
pip2 install requests
git clone https://github.com/p4kl0nc4t/Spammer-Grab
ls
chmod +x Spammer-Grab
ls
cd Spammer-Grab
ls
chmod 777 spammer.py

Всё готово, осталось только запустить наш бомбер этой командой:
python2 spammer.py --delay (пишем время задержки в сек, без скобок) --proxy (сюда пишем ссылку на прокси) и номер без +

Например:
python2 spammer.py --delay 5 --proxy http://177.35.25.32/ 7945314261234
Можно обойтись и без прокси, но тогда толку будет не особо много. Так что советую их использовать.
Есть бесплатные прокси, например https://awmproxy.com/freeproxy.php
Получаете ссылку оттуда и вставляете в Termux
Можете использовать платные прокси, тогда бомбежка будет просто адской.
И так у нас всё готово.
Чтобы остановить бомбёжку можно просто выйти из приложения.
Если захотите запустить несколько атак:
Делаете свайп в право и нажимаете New session.
Вводим:
cd Spammer-Grab
python2 spammer.py и сюда снова все параметры
Если закрыли Termux и хотим снова запустить бомбер делаем тоже самое:
cd Spammer-Grab
python2 spammer.py и сюда снова все параметры
В конце добавлю, на эмуляторах аднройда работать не будет, только на мобилах или Kali Linux.
