# Genshi AHK Flex v4.4

AHK скрипт для Genshin Impact

![hippo](https://media.giphy.com/media/xArjRR54nHdxJn8EG8/giphy.gif)

__Что по функционалу:__

- Рыбал'очка
- Бинд на интерактивную карту
- Оверлей с разной инфой
- Автоходьба
- Фастлут
- Скип диалогов
- Плавание
- Баннихоп
- Отключатель CGI кастсцен
- Макросы для лучников + драгонстрайки

__Возможности:__

- GUI c настройками
- ReShade
- Работа с реестром
- Автоматическая игра на "Лире ветров" (все сложно... но проще чем у других)
- Выбор режима имитации ввода SendInput, SendPlay, WinApi (по стандарту стоит SendInput)
- Ручной сброс настроек если скрипт не запускается "data\default.ahk"
- Вкладка безопасность: Name changer, Hash changer, WindowNameChanger, Random 15-40ms (NoMacro)

__Требования к правильной работе скрипта:__

- 60 FPS в игре
- Правильная установка Autohotkey
- Запуск от имени Администратора

:memo:__Показания к применению:__:memo:

1. Скачать и установить [Autohotkey.com](https://www.autohotkey.com/download/ahk-install.exe)

  "Custom installation" => "Unicode 64" => All checkboxes => "Install"
![hippo](https://media.giphy.com/media/LerrohpjasApOHH9G1/giphy.gif)

2. Скачать репозиторий (Code > [Download Zip👌](https://github.com/Kramar1337/GenshinImpact-AHK-flex/archive/main.zip))

3. Запустить "Genshi AHK Flex.ahk"

🎵 __Как подрубить лиру ветров:__ 🎵

1. Скачиваем и устанавливаем [Python](https://www.python.org/downloads/) 🐍

2. Запускаем батник в папке с скриптом "data\pip instal.bat", батник установит недостающие питонские библиотеки

3. Пылесосим пабчик в поисках интересных мелодий в формате .mid по следующим ссылкам 
- [Midistock](https://midistock.ru/) (топчик но не работает поиск по сайту)
- [Onlinesequencer](https://onlinesequencer.net/sequences) (норм поиск, но плохое качество)
- [Bitmidi](https://bitmidi.com/) (не пользовался, хз)

4. Понравившиеся мелодии закидываем в папку со скриптом где расположен файл "Genshi AHK Flex.ahk", позже файлы сами распределятся

5. Запускаем "Genshi AHK Flex.ahk", открываем GUI вкладка настройки

6. Удаляем предыдущие мелодии кнопка "Clear", Подгружаем новые мелодии кнопка "Parse", Запускаем питонский скрипт кнопка "Run"

7. Горячие клавиши Питонского скрипта: 

- Tab + ~(тильт или Ё) - Обновить список мелодий

- Tab + 1 2 3 4 5 6 7 8 9 0 - Воспроизвести мелодию на лире ветров

- Tab + Space - Остановить воспроизведение

🌈 __ReShade:__ 🌈

В решейде используется метод подмены файлов, скрипт перезаписывает решейд каждые 0.5 сек и через 15 сек переименовывает его, тупа обход в 4 строчки и инжекторы не нужны.

Очевидно эти манипуляции не безопасны и могут привести к блокировке.
1. Открываем GUI и выбираем вкладку ReShade
2. Нажимаем кнопку "Instal" и файлы из папки со скриптом скопируются в папку с игрой, путь к папке с игрой указан в "Settings"
3. Нажимаем кнопку "Run" и в течении 15 сек нужно запустить игру
- Home - Открыть ReShade меню
- Insert - Включить/отключить ReShade

🐠 __Рыбалка:__ 🎯

Как пользоваться:

Нажимаем 2 раза "X", закидываем удочку достаем рыбу и скрипт сам играет в эту коричневую мини игру с полосками. Как нарыбачились то нажимаем 1 раз "X" и авторыбалка остановится.

П.с. Тестировал на 1080p и 1440p мониторах на ультрах и минималках, + - норм робит... На данный момент отколиброван на слабую - среднюю рыбу, в "genConfig.ini" есть задержка "OptimizationFis=1" для максимальной скорости можно поставить "0" но сильно душит проц(3%) или поставить "50" но медленнее будет работать.

:musical_keyboard:__Горячие клавиши:__:musical_keyboard:
```
AHK
F1 - Карта
F2 - Оверлей
F3 - Автоходьба
F - Фастлут
Z - Скип диалогов
X - Авторыбалка (дабл клик вкл, сингл клик выкл)
N - Плавание
Space - Банихоп
Left - Пролистать оверлей
Right - Пролистать оверлей
End - Завершить работу скрипта
Page Up - *Приостановить-Возобновить работу скрипта
V - Macro Key
Numpad 0 - Включить/отключить банихоп
Numpad 1 - Стрельба на Amber по легиту но нужно быть в движении на +W
Numpad 2 - Стрельба на Fischl по легиту но нужно быть в движении на +W
Numpad 3 - Xiangling DragonStrike ?
Numpad 4 - Fischl и Amber рейдж +W
Numpad 5 - Venti Ganyu Yoimiya MachineGun
Numpad 6 - Klee Сombo
Numpad 7 - Diluc+Beidou DragonStrike
Numpad 8 - Noelle DragonStrike
Numpad 9 - Eula DragonStrike
Numpad + - Klee

Python
Tab + ~(тильт или Ё) - Обновить список мелодий
Tab + 1 2 3 4 5 6 7 8 9 0 - Воспроизвести мелодию на лире ветров
Tab + Space - Остановить воспроизведение

ReShade
Home - Открыть ReShade меню
Insert - Включить/отключить ReShade

Windows Shortcut
CTRL-ALT-Numpad0 - Запустить ярлык GenshAHK.lnk
```


<details>
<summary>==Список изменений==</summary>

Изменения: 09.09.2021
 - Скрыть надпись в тултипе рыбалочки

Изменения: 08.09.2021
 - Оверлей 4 стр, добавлен Тома
 - Оверлей 5 стр
 - Фикс скипа диалогов(они там что за моими скриптами следят? год все работало и вдруг отвал)
 - Еще 1 фикс рыбалки(3й по счету)
  
Изменения: 03.09.2021
 
 - Челы полоску с рыбалкой передвинули чи шо
 - Оверлей с рыбой-наживкой-спотами 8стр

Изменения: 01.09.2021

 - Уид хайдер не работал
 - Удалено ведьмачье чутье
 - Вместо него теперь рыбал'очка
 - Оверлей 5стр

Изменения: 30.08.2021
 - В фикс чат добавлен фастлут(фастлут не будет работать когда открыт игровой чат)
 - Подправил "Info" в трей меню
 - Рандомизатор рандомит 15-40мс(фастлут, бхоп, )
 - Другая иконка

Изменения: 29.08.2021
 - В трей добавлена кнопка создать ярлык игры с параметром запуска (-popupwindow) для игры в оконном без рамки(если не работает нужно Alt+Enter и перезайти)
 - Исправлены некоторые проблемы с интерактивной картой(и добавлены новые... проблемы)

Изменения: 28.08.2021
 - Возможность выставить в genConfig.ini дефолтный макрос DefaultJopaTrue=0
 - Добавлен Импорт настроек, старый genConfig.ini кидаем прям в окно скрипта и тот считает все настройки и перезапишет новый файл
 - Переделать оверлей 6стр(деревья)
 - На все хоткеи повесил "*" чтобы потоки не залипали(не забыть снять если чтото пойдет не так)
 - Подготовиться к рыбалке (скачать Рататуй?(механика рыбаловства 2004 года))

Изменения: 27.08.2021
 - Поправить оверлей 4стр(герои)

Изменения: 17.08.2021
 - Скип диалогов задержка срабатывания +70мс, сумарно 270мс

Изменения: 17.08.2021
 - Бинд на карту поддерживает многомониторную конфигурацию ПК, тестить некому так что хз как оно работает, в оконный без рамок идеально работает с ярлыком (-popupwindow) и реестр "Screenmanager Is Fullscreen mode = 0"

 - На SendInput режиме не работал макрос на стрельбу из лука на эмбер

 - Скрипт запускает сам себя от имени администратора если режим SendInput или WinApi

Изменения: 16.08.2021
 - Задержка срабатывания бхопа +15мс по дефолту
 - Добавлена возможность настроить задержку срабатывания "Бхопа"
 - Вернул старый оверлей стр 7

Изменения: 15.08.2021
 - Макросы мешают писать в чат, GUI"FIX Macro + chat" исправлено для "Плавание" и "Macro Key" DllCall"GetCursorInfo" Result1337 <> 0
 - Вернул джамп кансел на Klee "Numpad +"

Изменения: 14.08.2021
 - Кнопка приостанавливающая работу скрипта KEY"Page Up" шо это за кнопка? расположена рядом с кнопкой "Home"
 - Чекбокс "Максимальная скорость", если при работе скрипта игра лагает то снять галку и скрипт перейдет в медленный режим

Изменения: 12.08.2021
 - Изменено содержимое оверлея, стр 4 оружие и герои

Изменения: 10.08.2021
 
- Не работает автопуть с реестра, на релизе путь в одном месте в реестре, через год в другом, автопуть взял тут "UninstallString"
 
- Оверлей на ноутах с задушеным масштабированием? разрешением? плотностью пикселей? работает правильно, FIX Overlay Scale

Изменения: 04.08.2021
- Изменил темп сао опенинга в .mid(главное изменение этого патча) в FL Studio 20

Изменения: 02.08.2021
- RCS WinApi Bow, Двигать камеру вместе с макросом на нампад 4 и 5
- Переключение бхопа, бхоп мешает плавать на лодочке и кнопка "нампад 0" переключает бхоп вкл-выкл
- Исправил переключатель на карте, F1 стал умнее
- В трее добавил кнопку "Создать ярлык" которая биндит CTRL-ALT-Numpad0 для запуска ярлыка, хз почему но ярлык работает даже с неймченжером
- Мелкие исправления, шифт блочил работу кнопок, исправлено 2 кнопки

Изменения: 31.07.2021
- Добавлен драг анд дропс(перетаскивание) в GUI для песен лиры ветров

Изменения: 29.07.2021
- Фикс автоходьбы
- Изменил логику оверлея, кликабельные кнопки "листать оверлей" в гуи
- Почистил решейд
- Сделал дефолт ВинАпи режим ввода
- Переделал Гуи
- Не скрывать меню Гуи

Изменения: 05.2021
- Большая обнова изменено все
- Решейд
 
Изменения: 11.2020
- Фастлут
- Скип диалогов

==Конец списка==

</details>
🙏 Использование скриптов может привести к блокировке учетной записи, использовать на свой страх и риск.

🙈 Завтра VAC 🙉


Ps. Когда нибуть я научусь работать с [патернами](https://www.unknowncheats.me/forum/programming-for-beginners/171994-understanding-pattern-scanning-concept.html) и сделаю FPS Unlocker... когда это будет...
