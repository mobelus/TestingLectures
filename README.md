# TestingLectures
Lestures for testing courses


### ТИПЫ ТЕСТИРОВАНИЯ / ВИДЫ ТЕСТИРОВАНИЯ:

- Positive  - Позитивное тестирование (+)
- Negative - Негативное тестирование (-)

- Stress testing - Стрессовое тестирование

- Smoke Testing - Дымное тестирование – проверка на то, включится ли то, что тестируем и не загорится ли сразу (тест старта системы / кнопки ВКЛ)
- Бета тестирование – тестирование первого работающего прототипа полной версии программы с почти всем готовым функционалом

- Security Testing – тестирование возможно только, если что-то можно украсть - …
- Функциональное тестирование (-)(+) - 
- Тестирование методом Чёрного Ящика (-)(+) – 
- Тестирование методом Белого Ящика (-)(+) – 
- Компонентное / Блочное / Поблоковое тестирование (-)(+) - 
- Тестирование на производительноcть (-)(+) –

- Ручное тестирование (-)(+) – 
- Автоматическое тестирование (-)(+) – 
- Тест на соответствие документации (+) –
- Тестирование Графического интерфейса (-)(+) – 
- Тестирование на работу с входными данными (- некорректные)(+корректные) –
-- 

- Юзабилити тестирование (?) – Удобство использования тестируемого объекта -  Use –использовать  Ability – возможность 
- Тестирование на совместимость версий – 
- Регрессивное тестирование
- Интеграционное тестирование
- Валидация
- Верификация

- Тестирование на совместимость версий – 
```
Клиент (ver 1.0)  Сервер (ver 1.0) - было
Клиент (ver 2.0)  Сервер (ver 1.0) – стало
Вопрос, совместима ли версия клиента 2.0 с версией Сервера 1.0
Программа (ver 1.0)  конфигурационный файл (ver 1.0) - было
Программа (ver 2.0)  конфигурационный файл (ver 1.0) – стало
Вопрос, совместима ли версия Программы 2.0 с версией конфиг.файла 1.0
```

- Регрессивное тестирование – Проверка исправления вновь найденного дефекта
Проверка на то, не роняет ли разработанная сейчас фича, то, что работало ранее.

- Интеграционное тестирование – набор готовых, работающих друг с другом программ / модулей. И надо в их уже налаженную работу встроить ещё один уникальный новый модуль  


ТЕСТИРОВАНИЕ СОФТА:

ТЕСТИРОВАНИЕ СОФТА:

### ТЕОРИЯ ТЕСТИРОВАНИЯ - С ЧЕМ РАБОТАЕТ ТЕСТИРОВЩИК

План тестирования -  Очень общо описываются что тестируем, цели тестирования, общие положения. Описание методики тестирования продукта, на основании существующих к нему Требований (как должны работать те или иные части программы). То есть набор тест-кейсов, в неформализированном виде.

	Сценарий тестирования - (ТЕСТ КЕЙС /тестовый случай) ПРИСЛАТЬ ПРИМЕР
Их надо брать и описывать в Жире. И проходить по ним потом много раз. Их так же удобно потом передавать программисту или эксплуатации, чтобы они могли проверить работу той или иной части программы, к котрой написан тест-кейс. По сути, упрощенное описание теста. Входная информация, условий и последовательности выполнения действий и ожидаемого выходного результата. 
	Тестовые Входные данные - Наборы входных данных для тестов, а также ожидаемые результаты, с которыми полученные результаты выполнения тестов должны сравниваться как с эталонными.  Рекомендуется собирать вместе данные для каждой определенной группы тестов 
	Тестовый скрипт - Обычно говорят о программной реализации теста, хотя скрипт может описывать и ручные действия, необходимые для выполнения конкретного тест кейса. 
	Набор тестов - Как правило, сценарии тестирования объединяются в пакеты или наборы. Для группирования тестов со сходными задачами, или если надо менять порядок в группе тестов, поэтому их удобно хранить наборами.
	Результаты тестирования - Представляют собой суммарную информацию о прохождении тестов, Записываются и сохраняются для каждого этапа тестирования. 
(Тест-кейсы в табличке с плюсиками и минусиками.)
	Дефекты, Ошибки, Баги, Исключения,  - обнаруженные факты несоответствия системы предъявляемым требованиям. Порой их выписывают, делается градация, и типизпция Дефектов, чтобы в будущем понимать к какому виду отнёсся найденный дефект и оценка степени его критичности.
	



Любому тестировщику нужно 3 вещи:
- Ознакомиться с системой - в последствии знать систему и как она работает сейчас
- как должен работать какой-то новый функционал, чтобы понимать как его тестировать - СТАНДАРТНЫЕ СЦЕНАРИИ - то как ДОЛЖНО работать
- задаваться постоянно вопросом "ЧТО ЕСЛИ" и тестировать НЕСТАНДАРТНЫЕ СЦЕНАРИИ - то как МОЖЕТ работать, но не факт, что так ДОЛЖНО или вообще НЕ ДОЛЖНО

1. Ручное тестирование - примитивно, но тесты человеком порой необходимы даже самой хорошо запрограммированной системе, т.к. автот-тесты порой слишком "тупы", чтобы увидеть то, что может увидеть человек

2. Автотесты - Нужны только в тех случаях, когда чётко понятно, что тест или некая последовательность действий повторяется с минимальными изменениями.
Итеративный подход тестирования и архитектура на основе компонентов особенно подчеркивают целесообразность регрессионного тестирования качества продукта для каждого цикла компоновки. Все тесты, разработанные для версии X, являются потенциальными кандидатами для регрессионного тестирования версии X+1, X+2 и т.д. Когда тест повторяется несколько раз, возможно, его следует автоматизировать. Автоматизированное тестирование позволяет выполнять сценарии при повторном тестировании и переключать сотрудников на работу с тестированием новых функций

Для (Ручное тестирование / Автотресты) обоих важно ОДНО:

Важно соблюдать методологию тестирования
Чтобы ПО согласно Жизненному циклу разработки ПО шло строго по 5-ти пунктам:

1. Анализ требований
2. Проектирование
3. Разработка
4. Тестирование
5. Эксплуатация, Тех поддержка

ПРИЧИНА И ПРИМЕР: в жизни может произойти так: из 3-го этапа сразу в 5-тый.
Программист закодил фичу. Подумал, что закодил всё без ошибок.
Отдал заказчику, не стал из-за столь мелкой фичи беспокоить тестировщика.
Заказчик поставил прогу с Фичей, фича уронила ВСЁ приложение.

Ручные тесты - состоят из нескольких шагов, на каждом из которых тестер имеет возможность держать систему под контролем. Если мы зависли, ПО упало, мы увидели что-то на экране. Мы тут же можем пойти дальше и тестировать руками следуюший Кейс.
Т.Е. нам не обязательно 100% знать наперёд как работает тестируемый кусок ПО.

Автотесты  - стоят из последовательности шагов, на каждом из которых система может выйти из под контроля. Упасть, и тест не продолжится, зациклиться, зависнуть, и мы можем не понять это тест тупит или это ПО зависло. В этом случае, нам нужно будет переписывать и редактировать автотест, чтобы перейти к следующему Кейсу.
Т.Е. нам надо подробно знать или представлять на 99% как минимум как работает тестируемый кусок ПО, иначе автотест может не отработать никогда или мы будем править его 100 раз.

Автотесту нужно отдельно обрабатывать ситуацию и как-то мочь понимать, что ПО упало (он может сверится по Логам программы например), как правило автотест просто не способен отработать следующий после падения шаг. НО это далеко не факт. При ручном тестировании мы видим это сразу и нам не нужно дополнительно удостовериться в том, что программа работает некорректно.
ПЛЮСЫ и МИНУСЫ Ручного тестирования и Автотестов
Автотест не способен обработать НЕПРЕДВИДЕННЫЕ ситуации и шаги, которые в нём не описаны. Автотест никогда не поправит что-то докучи/заодно/заметил ещё. Ручное тестирование может обработать почти любое непредвиденное поведение программы, провести анализ и т.д. Ручное тестирование – человек может увидеть больше глазами и мозгом, и домыслить что-то более правильно, выявить неочевидное, поправит что-то докучи/заодно/что заметил ещё.

1. тестирование Фронт Энда
  Как правило тестирование верно реализованной логики согласно:
  БТ – Бизрнес Требование
  ФТ – Функциональным требованиям
  ТЗ / ЧТЗ – (Частное) Техническое Задание
  Документация / Спецификация
 Важно соблюдать методологию тестирования
 Чтобы ПО согласно Жизненному циклу разработки ПО шло строго по 5-ти пунктам:
  
2. тестирование Бэкэнда
 Через .bat-файлы. Скриптовые тесты. Тесты при помощи спец. программ.
 Бэкэнд это как правило СЕРВЕР. Для сервера проводится обычно НАГРУЗОЧНОЕ тестирование.
 Сколько сотен / тысяч / миллионов запросов в секунду и с какой интенсивностью сервер способен держать запросов. Как быстро он под нагрузкой способен работать и не УПАСТЬ. 
 ОБЫЧНО Консольные приложения, а значит всё управляется командами строчками
 Тестовый Стенд - Место / Среда / Виртуальная машина / Отдельный компьютер - на котором проводятся тесты. Это среда для тестирования Максмально приближенная к Среде в которой живёт и работает заказчик.
  
  ПРИМЕР: Заказчик работает на Windows 7, вся его компания и весь его парк машин в размере 200 ПК работает на 7-ке и ни на чём больше.  - Логично в качестве тестового стенда использовать виртуалку с 7-кой, и даже не тестить на Windows XP, MacOS или даже Win10. Ибо смысла мало.
  Другая ситуация, когда ПО кроссплатформенное, работать должно на разных версиях Винды, и не только на Винде - тогда тестовых стендов надо иметь несколько и тестироваться на многих тестовых стендах.



Бывают так же и наборы тестовых данных на которых ПО 100% падает.

```
Тест  - отчёт по каждому тесту - с описанием шагов внутри теста
Тест может пройти все шаги, и пройти успешно
Тест может свалиться на каком-то шаге и об этом надо 
```

Внутри Фреймворков для тестирования и автотестов
Есть уже какие-то определённые функции
Мы можем дополнять их и своими
Пользуемся функциями - и получаем ТЕСТ
ТЕСТ можно прогонять в Цикле несколько раз, с изменением каких-то параметров

ТЕСТИРОВАНИЕ User Interface.
SELENUIM (Web / Desctop), Bad Boy (Web / Desctop) - Через окно браузера: Веб драйвер имитирует действия человека.
1. Перешли на сайт
2. Найти кнопку с селектором, или каким-то названием
3. кликнуть на неё
4. вбить текст в эдит-бокс и т.д.

TEAM CITY - типа Дженкинс, но для Винды

CODE UI TEST - ТЕСТИРОВАНИЕ ВНУТРИ СТУДИИ
https://msdn.microsoft.com/en-us/library/dd286726.aspx


ТЗ по ГОСТ-у:
Как написать Техническое задание по ГОСТу | СЭД "Кодекс: документооборот" (kodeksdoc.ru)

ЧТО ДЕЛАЮТ ТЕСТИРОВЩИКИ В РЕАЛЬНОЙ ЖИЗНИ:
- пишут документы ТестКейсы, Тестпланы, ЧекЛисты (ТЗ и прочие документы, когда в компании не хватает рук или близится релиз, а тех.писатели не успевают с документами)
- продумывают тесты по ненаписанному ПО по ТЗ и пишут тесты по реализованному ПО
- тестеры тестируют ПО



### ТИПИЧНЫЕ ВОПРОСЫ ТЕСТИРОВЩИКУ:

КАК ВЫ БУДЕТЕ ТЕСТИРОВАТЬ:

- КАЛЬКУЛЯТОР
  - заставить его не работать
  - заставить его сломаться в рамках его функционала (вынуть батарейки это не сломать)
  - заставить его работать нестандартно, вызвать неопределённое поведение

в рамках известной корректной функциональности, заставить его сломаться или работать не так как ожидается.

- КАРАНДАШ, РУЧКА, КИРПИЧ
 - тестируется понимание функционального тестирования
 - тестируется понимание, что есть ГОСТы

- ОГНЕТУШИТЕЛЬ, ЛИФТ
 - как тестируется что-то что связанно с угрозой жизни человека

- МЕТЕОСТАНЦИЮ
 - тестируется умение фантазировать и придумывать нестандартные тесты для нестандартно описанной задачи
 - проявить изобретательность

Как тестировать Карандаш, тостер, банкомат, мост, аппарат проающий бутылки воды
https://www.youtube.com/watch?v=Erctsy6i0zo

### ТИПИЧНЫЕ ВОПРОСЫ ТЕСТИРОВЩИКУ:

Как тестировать Карандаш, тостер, банкомат, мост, аппарат проающий бутылки воды
https://www.youtube.com/watch?v=Erctsy6i0zo


1. Просим - есть ли СПЦИФИКАЦИЯ.
2. Уточнение 
2.1 всех внутренних свойств тестируемого объекта (исходное состояние того, что мы тестируем)
2.2 всех внешних условий среды, в которых предполагается выполнять сами тесты (среда тестирования)
3. Начинаем с позитивного тестирования. (Предмет теста выполняет те функции, к которым он был предназначен, для чего был изначально сделан)
4. Негативное тестирование потом, возможно.

// Закзик Внешний заказчик / Внутри

ТЕОРИЯ: Должна быть написана документация на основе требований от заказчика 
(Работы заказчика / бизнес-аналитика / менеджера в нашей компании, который работает с заказчиком и / аналитика на нашей стороне)

ИДЕАЛ ТЕОРИИ / КАК ТЕОРИЯ ВИДИТ СЕБЯ НА ПРАКТИКЕ: 
[1] Заказчик говорит в общих чертах что нужно, составляет DOC-домунет в который вставляет  принтскрины из разных программ, которые ему нравятся, с функционалом примерно похожим на тот, что ему реально надо, и дописывает к этим принскринам 
свои комментарии, что доделать / поправить / изменить и т.д.
ИЛИ на софт такого типа (РЖМ/МЕДИЦИНА/ГОСОРГАНЫ/СТРОИТЕЛЬСТВО) есть ГОСТЫ, СНИПЫ, и прочее, и заказчик копирует описание из ГОСТОВ.
[2] Наш менеджер записывает заказчика на диктофон, чтобы запомнить все его котелки, допечатывает DOC-файл от заказчика поадекватнее, дописывает подробности, которые заказчик произнёс вслух, но не дописал в файл текстом. Проверил документ на здравый смысл и уточнил у заказчика, пункты, которые сделать физически невозможно или если написан полный бред, обсудил его, чтобы бред устранить на первом же этапе согласования. +оформляет документ по ГОСТУ, если он знает ГОСТ.
[ПО ГОСТУ – ПРИСЛАТЬ ДОК ОФОРМЛЕННЫЙ ПО ГОСТУ]
[3] Это всё попадает Аналитику - Аналитик в спец программе рисует интерфесы, убирая "принтскрины-примеры", описывает как общее:
структура приложения / основные функуиональные блоки

ПРАКТИКА 1: Документация пишется от балды, но хоть какая-то черновая, дописывается по готовому и оттестированному Софту.

ПРАКТИКА 2: Документация пишется по уже написанному, готовому и оттестированному Софту, за 5 дней до передачи заказчику.



###  НЕМНОГО О СКПРИТАХ

Writing C++ Scripts
 Applies to TestComplete 12.31, last modified on July 10, 2017
C++Script is a specific dialect of the C++ programming language supported by TestComplete. It is based on JScript. It was specially designed to let C++ developers easily port script routines to their C++ Self-Testing and Connected Applications.
TestComplete can both record and play back C++Script routines. That is, you can record a script in TestComplete, debug it there, then import this script to your C++ application and make it work by adding just a few lines. For instance:
// This code was recorded by TestComplete:
```
function Test()
{
  var p, w;
  p = Sys["Process"]("notepad");
  w = p["Window"]("Notepad", "*");
  w["Activate"]();
  w["Window"]("Edit")["VScroll"]["Pos"] = 0;
  w["Window"]("Edit")["Click"](9, 9);
  Sys["Keys"]("Test");
  w["MainMenu"]["Click"]("File|Exit");
}	// This code was imported to a C++ Connected Application:
 
#include "c:\TestComplete\Connected Apps\C++\script.h"
using namespace TestComplete;
IMPLEMENT_TESTCOMPLETE_GLOBAL_OBJECTS
```

```
function Test()
{
  var p, w;
  p = Sys["Process"]("notepad");
  w = p["Window"]("Notepad", "*");
  w["Activate"]();
  w["Window"]("Edit")["VScroll"]["Pos"] = 0;
  w["Window"]("Edit")["Click"](9, 9);
  Sys["Keys"]("Test");
  w["MainMenu"]["Click"]("File|Exit");
}
The language of the code recorded by TestComplete for your C++ projects is JScript. So, you can simply write anything that is allowed in JScript and this script will be operational. For instance, in JScript and C++Script all variables and constants are VARIANT. You must declare them and you should do this using the following format:
var p, w;
Syntax of C++ scripts is the same as the syntax of C# scripts (since C#Script is also based on JScript). They are the same as long as the scripts reside in TestComplete. If you export scripts to a Connected Application, they will be different. That is, the syntax of C++Script and C#Script routines exported to C++ and C# Connected and Self-Testing Applications will differ.
Once again, the idea of having C++Scripts as a separate script language for TestComplete projects is to let developers, who are used to C++, write script code that requires minimal changes when being imported into C++ applications. When writing such code in C++Script, please keep in mind the following rules, which distinguish C++Script from JScript:
1.	When calling methods, use only the following notation: method names are quoted and placed in brackets, and their parameters are placed in parentheses:
C++Script
Log["Message"]("My Message", "My Message Description", 0, 1);
```


ТЕСТЫ БЫВАЮТ

МОДУЛЬНЫЕ
 - Тестирование отдельного модуля, без привязки к целостной системе ПО

ИНТЕГРАЦИОННЫЕ
 - Как новая хотелка от заказчика встроится в существующую инфраструктуру (ПО) 
- Тестирование того, как новая фича въедет в уже существующее ПО - Тестирование модуля при взаимодействии с другими уже существующими модулями, чтобы проверить на сколько он в состоянии функционировать с другими частями и модулями ПО, не ломая работу других.

ПРИЁМОЧНЫЕ
 - Проверка конечной работы продукта перед передачей заказчику - Перед передачей заказчику проверяется, чтобы заказчику был передан код программы, и чтобы заказчик мог бы собрать проект у себя.




Дженкинс нужен для 

contiues Integration

автосбока

автокомпиляция 

Код закодили.
Его выкачивают через гит из ветки.
его компилят компилятором, или несколькими компиляторами
потом запускаются юнит тесты (юнит тесты пишутся разработчиками)



Понимание жизненного цикла ПО, разработки, тестирования

Роль тестирования в жизненном цикле разработки ПО
В первую очередь стоит отметить, что процесс тестирования ПО тесно связан непосредственно с процессом разработки.


### Жизненный цикл разработки состоит из следующих этапов:

1. Анализ требований
2. Дизайн
3. Разработка
4. Тестирование и дебаггинг
5. Эксплуатация и поддержка

https://xbsoftware.ru/blog/zhiznennyj-tsykl-testirovaniya-po-preimuschestva-shagi/

ПОЧЕМУ ТАК ВАЖНО следовать Жизненному циклу ПО:
ПРИЧИНА И ПРИМЕР: в жизни может произойти так: из 3-го этапа сразу в 5-тый.
Программист закодил фичу. Подумал, что закодил всё без ошибок.
Отдал заказчику, не стал из-за столь мелкой фичи беспокоить тестировщика.
Заказчик поставил прогу с Фичей, фича уронила ВСЁ приложение.

### Жизненный цикл Тестирования
Жизненный цикл тестирования наилучшим образом реализуется как процесс со многими итерациями. В каждом цикле итераций коллектив разработчиков программного обеспечения создает промежуточную версию компоновки, которая является потенциальным кандидатом для тестирования.
Цели и акценты разработчиков меняются в разных циклах итерации. Согласно этому должны строить свои планы и участники коллектива тестирования. Мы рекомендуем ограничивать до минимума усилия по планированию, а там, где они необходимы, привязывать их точно ко времени, когда они потребуются. Также мы рекомендуем планировать тестирование только для ближайшей итерации.
Для каждой компоновки в тесты будут вноситься добавления и уточнения, и что-то будет удаляться. Некоторые из тестов будут неизменными и будут включаться в комплект тестов, применяемый при тестировании каждой компоновки в жизненном цикле. При таком подходе тесты изменяются и уточняются, как и само программное обеспечение. Нет никакой фиксированной спецификации программного обеспечения, и сами тесты тоже не фиксированы. На рисунке показана схема развития тестов во времени.
Этот подход на основе итераций и архитектура на основе компонентов особенно подчеркивают целесообразность регрессионного тестирования качества продукта для каждого цикла компоновки. Все тесты, разработанные для версии X, являются потенциальными кандидатами для регрессионного тестирования версии X+1, X+2 и т.д. Когда тест повторяется несколько раз, возможно, его следует автоматизировать. Автоматизированное тестирование позволяет выполнять сценарии при повторном тестировании и переключать сотрудников на работу с тестированием новых функций.
Рассмотрим только жизненный цикл тестирования, пока не обращая внимания на остальные части проекта. На рисунке показана структура различных задач дисциплины тестирования в заданной итерации.

Основные артефакты тестирования


Знание методик тестирования;




Автоматическое тестирование ПО

ручное тестирование ПО

Подготовка тест планов - тест кейсы

автотесты - 

Написание модульных  автотестов
интеграционных автотестов
приемочных автотестов


Работа с тестовой документацией (Zephyr);

Работа в багтрекинговой системе (JIRA);

Работа с документацией (Confluence).

Требования
Высшее образование;

Опыт от 1 года в области тестирования;

Знание методик тестирования;

Базовые знания с++;

Базовые знание SQL;

Умение разбираться в чужом коде;

Понимание жизненного цикла ПО;

Желателен опыт работы с заказчиком;

Личностные качества: аккуратный, активный, инициативный, исполнительный, коммуникабельный, обязательный, ориентированный на результат, ответственный, работоспособный, самостоятельный.





### HOTKEYS
```
Найти Во всём проекте
Ctrl + Shift + F
Ctrl + H   заменить много где во всём файле
Alt - Горизонтальное выделение квадратом и редактирование Квадратом
Ctrl + Shift + Left / Ctrl + Shift + Right

Alt + Tab
Alt + F4

Ctrl + F
Crtl + L - Перейти к адресной строке проводника или Internet Explorer.
F5 - Обновить окно проводника или Internet 
Backspace -	Перейти на уровень вверх в окне проводника или Internet Explorer.

F2 - переименовать файл / папку
Выдекление  / Перетаскивания с Shift / Ctrl

Insert !!!
Перехлж нра цифровую клаиватуру Num Lock !!!

Ctrl + A
Ctrl + C
= Ctrl + V
= Shift + Insert
Ctrl + X
Ctrl + S
Ctrl + Z

Ctrl + Shift + Del
Ctrl + Shift + Escape

Alt + Tab
Ctrl + N
Ctrl + Shift + N

Win + E
Win + Pause
Win + L

Switch between CPP and H
MSVS:	Ctrl + K + O 
Qt:		F4
Win commands
Win + R
```

### WIN COMMAND LINE COMMANDS
```
cmd
notepad
mspaint
calc
explorer
inetmgr
services.msc
regedit
powershell
msconfig
diskmgmt.msc
```

### Git / Svn commands
```
+ clone - склонировать репозиторий - клонировать
+ add - добавить файлы к коммиту - добавить
+ commit - зафиксировать изменения - зафиксировать
+ pull - затянуть с сервера - тянуть
+ push - загрузить на сервер - толкать

* branch - создать новую ветку  - ветка / ответвление
* merge - слиться с какой-то веткой / слить свою ветку с чье-то - слияние
* checkout - перейти на ветку - проверить
* revert
* rebase
* fetch

status
log
reset
remote
stash
```

```
git config --global user.email "you111@mail.com"
git config --global user.name "You111"

git add (имя файла в котором произошли изменения)
git add index.html - файл в котором были изменения в примере

git commit -m "comment 3"


Закомитить изменения у себя - делается в дыва шага
1. git add
2. git commit -m "(комментарий)"

Отправить изменения на сервер git push
Получить изменения с сервера git pull

Вывести весь список доступный веток
git branch -a

Перейти в ветку
git checkout (имя ветки)

Создать новую ветку
git branch (имя ветки)

Загрузить себе все изменения которые произошли во всех ветках,
но не произойдет гир пул (в ветку на которой мы сейчас находимся 
не загрузится ее последнее состояние (последний коммит)
git fetch


git merge (ветка которую мы хотим влить в себя)


git clone ИМЯ_РЕПОЗИТОРИЯ

git add ФАЙЛ_С_ИЗМЕНЕНИЯМИ
git commit -m "COMMENT"

git push
git pull
```


### English 
```
new [нью] - новый
old [олд] - старый
size [сайз] - размер
next [некст] - следующий / Далее
back [бэк] - назад / спина
previous [привэос] - предыдущий
data [дэйта] - данные
add [эд] - добавить
delete [делит] - удалить
step [стэп] - шаг
open [оупэн] - открыть
close [клоуз] - закрыть
save [сейв] - сохранить
load [лоад] - загрузить
option [опшн] - настройка, опция, вариант
propertie [проперти] - свойство
download [даунлоад] - скачать
upload [аплоад] - загрузить

who ? [ху] - кто
what ? [уот] - что
when ? [уэн] - когда
why ? [уай] - полчему
how ? [хау] - как
whom ? [хум] - кому
about [эбаут] - о (чём-то / ком-то)

and [энд] - и
bool [бул] - булева
break [брэйк] - разбить
case [кейс] - случай
catch [кеч] - поймать / ловить
character [чарактэр] - символ, персонаж
cast [каст] - перевести (выполнить перевод из одного сосот. в другое)
continue [континью] - продолжить
default [дефолт] - стандартный / по умолчанию
delete [делит] - удалить
do [ду] - делать
double [дабл] - двойной / удвоенный
dynamic [дайнэмик] - динамический
else [элс] - иначе
export [экспорт] - экспортировать
extern [экстерн] - внешний
false [фолс] - ЛОЖЬ
float [флоат] - 
for [фор] - для
go to [гоу ту] - идити в
if [иф] - если
integer [интеджер] - целое (всмысле не дробное, про число)
name [нейм] - имя
space [спейс] - пробел, пространство
new [нью] - новый
pointer [поинтер] - указатель
private [прайвет] - приватный
protected [протектед] - защищённый
public [паблик] - публичный
return [ретёрн] - вернуть
short [шорт] - короткий
sign [сайн] - знак
signed [сайнт] - знаковый
size of [сайз оф] - размер (чего-то)
structure [страчер] - структура
switch [свич] - переключиться
template [темплейт] - шаблон
this [Зис] - это
thread [тред] - поток
local [локал] - локал
throw [фроу] - бросать
true [тру] - ИСТИНА
try [трай] - попытаться
type [тайп] - тип
union [юнион] - объединение
unsigned [ансайнт] - беззнаковый
use [юз] - использовать
using [юзинг] - используя
while [уайл] - во то время как

function [фанкшн] - функция
jump [джамп] - прыгать
big [биг] - большой
small [смол] - маленький
little [литл] - маленький
edit [эдит] - менять
deny [денай] - отменить
enable [энейбл] - задействовать
deprecated [деприкэйтед] - 
call [кол] - вызвать, вызов
substract [сабстракт] - 
multiply [мультиплай] - 
erase [ирэйз] - 

add [эд] - 
insert [инсерт] - вставить
select [селект] - выбирать
new [нью] - создать

complete [комплит] - 
incomplete [инкомплит] - 
different [дифферент] - 
difference [дифференс] - 
algorythm [элгоритм] - 
compare [кмпэар] - 
read [рид] - 
write [райт] - 
access [эксэс] - 
word [ворд] - 
last [лэст] - 
first [фёрст] - 
begin [бегин] - 
end [энд] - 
create [криэйт] - 
destroy [дестрой] - 
total [тотал] - 
location [локэйшн] - 
recent[рисэнт] - 
print [принт] - 
all [ол] - 
both [боуф] - 
side [сайд] - 
letter [лэттэр] - 
preview [привью] - 
attach [эттач] - вложение
share [шэр] - 
Save [сэйв] - 
load [лоад] - 
change [чейндж] - 
support [сапорт] - 
tool [тул] Инструмент - 
Check [чек] - 
Paste [пэйст] - Вставить
Cut [кат] - Вырезать
Font [фонт] - Шрифт
Color [колор] - Цвет 
Show [шоу] - 
Increase [инкриз] - 
Decrease [дериз] - 
Change [чейндж] - 
Find [файнд] - 
Replace [реплэйс] - 
Select [селект] - 
Shape [шэйп] - 
Blank [блэнк] - Пустая 
Link [линк] - Ссылки
Header [хэдэр] - заголовок
Equation [экуэйжн] - 

Margin [маргин] - Поле
Page [пэйдж] - Страница
Line [лайн] - строка
Column [колам] - столбец
Column [колам] - Колонка
Even [ивэн] - Четная
Odd [од] - Нечетная
Left [лэфт] - Слева
Right [рфйт] - Справа
Before [бефор] - До
After [афтэр] - После 
Position [позишн] - Положение
Bring [бринг] - принести
Forward [форворд] - вперед
Backward [бэкворд] - назад 
Send [сэнд] - отправить 
Pane [пээн] - Область
Align [элайн] - Выровнять
Rotate [ротэйт] - Повернуть
angle [энгл] - угол
Mark [марк] - Пометить
Entry [энтри] - элемент
Note [ноут] - Показать сноски
Style [стайл] - Стиль
List [лист] - 
Rule [рул] - Правила
Field [фиилд] -  поле
Merge [мёрдж] - объединить
Split [сплит] - Разделить 

help [хэлп] - помогите, помогать, помощь
tab [тэб] - вкладка
home [хоум] - дом
push [пуш] - нажать, давить
page [пэйдж] - страница
reference [референс] - ссылка
mail [мэйл] - почта
view [вью] - вид, представление
review [ревью] - обзор
title [тайтл] - надпись
point [поинт] - точка
button [баттон] - кнопка
box [бокс] - 
scroll [скрол] - Ползунок
scroll box [скрол бокс] - Ползунок прокрутки
zoom [зум] - прибилжать
send [сэнд] - отправлять
recieve [ресив] - получать
layout [лэйаут] - 
label [лэйбл] - надпись
save [сэйв] - сохранить
save as [сэйв эз] - сохранить как
open [оупен] - открыть
close [клоуз] - закрыть
info [инфо] - сведения
recent [рисэнт] - последние
print [принт] - печать
options [опшн] - параметры
exit [экзит] - Выход

Window [уиндоу] - окно
Comment [коммент] - Примечание, Комментарии
Change [чейндж] - 
Accept [эксэпт] - 
Protect [протэкт] - 
Block [блок] - 
Restrict [рестрикт] - 
Record [рекорд] - 
Security [секьюрити] - 
Drop [дроп] - 
Pick [пик] - 
Frame [фрэйм] - рамку 
Reset [рисэт] - 
Image [имэйдж] - 
Mode [моуд] - Режим 
Group [груп] - Группи
Schema [шэма] - Схема
Template [тэмплейт] - Шаблоны
Border [бордэр] - Границы
Pen [пэн] - перо
Style [стайл] - Стиль 
Weight [вэйт] - Толщина 
Height [хэйт] - Высота 
Widht [уидт] - Ширина 
Draw [дроу] - 
Table [тэйбл] - Нарисовать таблицуэ
Eraser [эрэйзр] - Ластик
Fit [фит] - Автоподбор
Align [элайн] - Выровнять 
Repeat [рипит] - Повторить 
Convert [ковёрт] - Преобразовать 
Adjust [эджаст] - 
Background [бэкграунд] - 
Reset [рисэт] - 
Compress [компрэс] - 
Wrap [урэп] - 
Arrange [эррэйндж] - 

Layout [лэйаут] -  Макет 
Crop [кроп] - Обрезка

Forward [форвуард] - 
Backward [бэквуард] - 
Fill [фил] - 
Outline [аутлайн] - 
Direction [дайрекшн] - 
Shape [шэйп] - Фигуры
Picture [пикчэр] - Рисунок
Axe [экс] - Оси
Wall [уол] - Стенка
Area [эриа] - Область
Background [бэкграунд] - Фон
Up [ап] - 
Down [даун] - 
under [андэр] - 
over [оувэр] - 
Error [эррор] - 
exception [эксэпшн] - 

point [поинт] - 
line [лайн] - 
polyline [полилайн] - 
ellipse [эллипс] - 
circle [сиркл] - 
rectangle [рэктэнгл] - 
square [скуэар] - 
triangle [трайэнгл] - 
angle [энгл] - 
side [сайд] - 
polygon [полигон] - 

select [селект] - 
insert [инсерт] - 
update [апдейт] - 
delete [делит] - 

include [инклуд] - 
import [импорт] - 
return [ретёрн] - 

memory [мэмори] - 
drie [драйв] - 
sound [саунд] -
unique [юник] - 
description [дескрипшн] - 
display [дисплэй] - 
launch [лаунч] - 
crash [скэр] - 
fall [фол] - 
settings [сэттингз] - 
amount [эмаунт] - 
must [маст] - 
disable [дисэйбл] - 
prefear [прифэар] - 
count [каунт] - 
engine [энджин] - 
core [кор]
current [каррэнт]
device [девайс]
brows [брауз]
advanced [эдвансд] - дополнительно
direct [дайрект]
custom [кастом] - определённая
сompatibillity [компатибилити] - 
show [шоу] - 
with [уизтх] -
specify [специфити] - 
present [презент]
allow [эллау]
any [эни]
```


