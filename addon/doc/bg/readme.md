# Навигационен режим на цифровия блок (Numpad Nav Mode) #

* Автор: Luke Davis (Open Source Systems ООД)
* Изтегляне на [стабилна версия][1]

"Навигационен режим на цифровия блок" е добавка за
[NVDA](https://nvaccess.org/), която ви позволява лесно да превключвате
цифровия блок на клавиатурата между режима му на работа при включен NVDA и
нормалния му режим на работа без работещ екранен четец. Това може да бъде
особено полезно за потребители, преминаващи от JAWS към NVDA. Тази добавка
също дава гъвкав контрол върху превключването на клавиша Num Lock, както при
стартиране на NVDA, така и по избор посредством конфигурационните профили.

### Разяснение и характеристики на режимите на навигация

Нормалните функции на цифровата клавиатура на компютъра с изключен Num Lock
са: Page Up, Page Down, Home, End, четири стрелки за движение нагоре,
надолу, наляво и надясно и клавиш Delete. Но NVDA напълно прихваща цифровия
блок, за да осигури клавиши за преглед, управление на мишката и клавиши за
навигация по обекти. Това е така дори при използване на клавиатурна подредба
за лаптоп, което дублира тези функции на клавиши, които не са част от
цифровия блок, за случаите в които не е наличен цифров блок.

Някои потребители обаче разполагат с цифров блок на своя лаптоп и биха
предпочели да го използват за навигация в Windows, особено когато някои
лаптопи не разполагат с Home, End или други подобни клавиши. Това са част от
случаите, в които тази добавка може да помогне. Освен това, някои
потребители на настолни компютри понякога може да предпочетат да използват
цифровия блок за тези функции на клавиатурата вместо стандартните клавиши,
което тази добавка позволява. Това включва популярната команда на JAWS
Insert от цифровия блок+2 от цифровия блок, за прочитане на всичко, което
беше конкретна заявка за функция от някои ранни потребители на тази добавка.

### Как работи

При изключен Num Lock, без значение коя клавиатурна подредба се ползва, тази
добавка ще ви позволи да натиснете Alt+NVDA+Плюс от цифровия блок (който
обикновено е дългият клавиш втори подред от долу нагоре в десния край), за
бързо и лесно превключване между нормалната навигация на NVDA и класическите
команди за навигация на Windows. Тази клавишна команда може да бъде
променена в диалоговия прозорец "Жестове на въвеждане", в категорията
"Въвеждане".

Имайте предвид, че тази добавка не забранява използването на Insert от
цифровия блок като модификатор на NVDA, ако сте указали да е така. Ако
искате тази функция, моля, уведомете ме, въпреки че можете ръчно да
изключите Insert от цифровия блок като модификатор в настройките на
клавиатурата на NVDA. Също така не променя функцията на NVDA с Delete от
цифровия блок (клавишът между нула и Enter) – свържете се с мен, ако желаете
такава функция.

Ако предпочитате да стартирате NVDA с активен по подразбиране навигационен
режим на Windows, можете да конфигурирате това в настройките на NVDA. От
менюто на NVDA изберете "Настройки" и след това "Опции" и намерете панела за
настройки на добавката "Навигационен режим на цифровия блок". Там ще можете
да поставите отметка, с която да укажете навигационния режим на Windows да е
активен по подразбиране при стартиране на NVDA. За да стигнете бързо,
натиснете NVDA+N -> Н -> О, след това Н един или няколко пъти, докато не
чуете "Навигационен режим на цифровия блок".

### Функции на Num Lock

По подразбиране нищо не се прави с клавиша Num Lock.

Ако споделяте компютъра си със зрящ потребител, който предпочита Num Lock
винаги да е включен, но вие предпочитате да е изключен, така че цифровият
блок да работи с NVDA, може да искате Num Lock да се изключва автоматично
при стартиране на NVDA. Друг вариант е, ако въвеждате много данни, да
предпочитате Num Lock винаги да е включен когато стартирате NVDA.

Отидете в менюто на NVDA -> Настройки -> Опции -> Навигационен режим на цифровия блок и използвайте селектора "Състояние на Num Lock при стартиране на NVDA или зареждане на профил". Там има три опции:
Първата, "Без промяна", е по подразбиране и няма да засяга Num Lock. Той ще бъде в състоянието, в което е бил преди стартирането на NVDA.
Втората опция е "Изключване на Num Lock", която винаги ще изключва NumLock, когато NVDA стартира.
Третата опция, "Включване на Num Lock", ще включи numlock, ако при стартиране на NVDA е бил в изключено състояние.
Ако изберете втората или третата опция, при изход от NVDA, Num Lock ще бъде възстановен до състоянието, в което е бил преди това. Например, ако изберете "Изключване на Num Lock" и Num Lock при стартиране на NVDA е бил включен, той ще бъде изключен докато използвате NVDA, но ще бъде включен отново, при изход от NVDA.

#### Специални случаи на употреба

Ако използвате конфигурационните профили на NVDA и искате Num Lock да се
включва автоматично, когато се задействат определени профили, направете
следното:

* Докато сте в профила "Обичайни настройки", отидете на панела с настройки
  на "Навигационен режим на цифровия блок", описан по-горе. Поставете
  отметка в полето "Първоначалното състояние на Num Lock зависи от
  конфигурационния профил". Тази опция по подразбиране не е включена.

* Задействайте бутона "OK".

* Превключете на профила, в който искате Num Lock винаги да бъде изключен
  или включен.

* Върнете се в панела с настройки на "Навигационен режим на цифровия блок" и
  задайте опцията за включване/изключване на Num Lock, както предпочитате.

* След това задействайте бутона "OK". Сега, когато се задейства този профил,
  Num Lock автоматично ще се промени в желаното състояние.

Имайте предвид, че това е нова функция и не знам дали някой има полза от
нея. Ако намерите такава, моля, пишете ми или [пуснете
доклад](https://github.com/opensourcesys/numpadNavMode/issues/new), за да ми
споделите.

### Нови възможности

Окуражавам ви да [пуснете
доклад](https://github.com/openSourceSys/numpadNavMode/issues/new) или да ми
пишете на е-пощата с всякакви предложения за функции или други начини на
използване на добавката, които не съм изброил тук, или просто да ме
уведомите, че добавката ви е от полза!

### История

Тази добавка е пряк резултат от искания от страна на потребителите, на които
съм попадал през годините и дискусия в GitHub в [доклад
#9549](https://github.com/nvaccess/nvda/issues/9549). Благодарности на
@Qchristensen и @feerrenrut. Основното изпълнение на функциите на numlock е
заимствано от остарялата добавка NumLock Manager от Noelia Ruiz (@nvdaes в
GitHub) и други. Използва се с разрешение.

### Списък с промените

Този списък с промените е непълен. Вижте Git log за повече подробности.

* 23.0: Съвместимост с NVDA 2023.X.

* 23.1.0: Добавена е функция за управление на Num Lock. По-добро
  протоколиране. Подобрено управление на конфигурационните профили (WIP).

[[!tag dev stable]]

[1]: https://addons.nvda-project.org/files/get.php?file=numpadNavMode