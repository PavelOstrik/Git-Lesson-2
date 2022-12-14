Создаём папку, на рабочем столе к примеру, открываем её в Visiual Studio Cod, далее если мы хотим, чтобы её начало отслеживать git вводим в терминале  Visiual Studio Cod команду:    
  **git --version** - приписывает к нашей папке git
  
  **git init** - теперь git в этой папке начинает отслеживать изминения, себя можно проверить, открыть папку, там должна появиться скрытая папка .git
  
Чтобы открыть терминал в Visiual Studio Cod заходим в Вид - Терминал

**git status** - чтобы узнать подробности о папке, например прошло ли сохранение или выдаст список версий сохранений 

Создаём новый файл в папке, называем его, расширения обязательно указываем

**Ctrl + S** - сохранение внутри файла, если в названии файла стоит белая точка, это значит, что он не сохранен.

Untracked Files - нет отслеживаемых файлов

**git add "File name"** - добавить файл, который нужно отследить, кнопка Tab дозаполнит имя файла по первым 2 буквам

Changes to be commited - некоторые изменения могут быть сохранены

**git commit -m "Comment"** - Сохраняем с добавлением комментария. commit - сохранять

**git log** - журнал изминений, выдаст все версии файла

Работаем в самом файле, что-то написали, сохраняем написанное Ctrl + S, далее чтобы git сохранил изменения пишем git add "File name", а уже далее добавляем комментарий с сохранением git commit -m "Comment"

**git checkout "Name version"** - перейти к предыдущей версии/сохранению, достаточно ввести первые 4 знанка имени версии

**git checkout master** - продолжить работу с актуальной версией

**git diff** - разница между м/у текущим состоянием файла и сохраненным

Стрелкой вверх можно вывести ранее используемые команды 

Git следит за файлом по наименованию, и если мы его переименовали, то git будет считать, что мы удалили предыдущее название, далее нужно сохранить новый файл. git add, далее git commit -m

# Синтаксис языка MarkDown

## Заголовки

## **Выдлеление текста**

Markdown воспринимает звёздочки «*» и символы подчёркивания «_» как признаки смыслового выделения текста:

    * Текст, окружённый одиночными «*» или «_», будет заключен в HTML-тэг <em>.

    * Текст, окружённый двойными «*» или «_», будет заключен в HTML-тэг <strong>.

Иными словами, текст, окруженный одинарными символами, выделяется курсивным шрифтом, а текст, окруженный двойными символами, выделяется полужирным шрифтом. Также, выделенный фрагмент может находиться в любой части слова. Текст, выделенный курсивом с использованием синтаксиса языка Markdown, выглядит следующим 
образом:

### *Курсив* - обозначение курсива

### **Полужирный** - выделение текста

### ***Полужирный Курсив***

Или

_Курсив_

__Полужирный__

 Пере___распред___деление

 ___Полужирный курсив___

## **Списки**
Ненумерованный список
* Элемент 1
* Элемент 2

- Элемент 1
- Элемент 2

+ Элемент 1
+ Элемент 2

Нумерованный список
1. Элемент
2. Элемент
3. Элемент

## **Цитаты**

    >Это пример цитаты

    >в которой перед каждой строкой

    >ставится угловая скобка.

Вложение цитаты в цитату выглядит следующим образом: 

    > Первый уровень цитирования
    >> Второй уровень цитирования
    >>> Третий уровень цитирования
    >
    >Первый уровень цитирования

Цитата, вставленная в список, выглядит следующим образом:

    1. Элемент списка с цитатой:

    > Это цитата
    > внутри элемента списка.

    2. Второй элемент списка

 При вставке цитат в элементы списка важно учитывать, что элементы списка должны находиться на одном уровне, а цитаты должны указываться с отступом. В случае, если правило с единым уровнем списка не соблюдается, следующий после цитаты элемент списка будет автоматически нумероваться цифрой «1.». Кроме того, при необходимости в список можно вставить исходный код. В этом случае его нужно писать с двойным отступом – 8 пробелов или 2 символа табуляции.

    * Элемент списка, содержащий исходный код

       <исходный код >

## **Блоки кода**

Отформатированные блоки кода используются в случае необходимости процитировать исходный код программ или разметки. Для создания блока кода в языке Markdown необходимо каждую строку параграфа начинать с отступа, состоящего из четырех пробелов или одного символа табуляции. Блок кода продолжается до тех пор, пока не встретится строка без отступа (или конец текста). Внутри блока кода амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в элементы HTML разметки. Кроме того, следует отметить, что внутри блоков кода обычный синтаксис Markdown не обрабатывается. Блок кода в Markdown выглядит следующим образом:

Это обычный параграф:

    Это блок кода  

## **Горизонтальные линии (разделители)**

Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. Горизонтальные линии в Markdown выглядят следующим образом:

    Первая часть текста, который необходимо разделить
    ***
    Вторая часть текста, который необходимо разделить

Или

    Первая часть текста, который необходимо разделить

    ---

    Вторая часть текста, который необходимо разделить

При использовании данного инструмента важно помнить, что после первой части текста и перед второй необходимо оставлять пустую строку. Данное правило необходимо соблюдать только при использовании дефисов. Если его не соблюдать, на экран будет выведен заголовок второго уровня и строка обычного текста. При использовании символа звездочки данным правилом можно пренебречь.

## **Строчные элементы**

### **Ссылки**

Markdown поддерживает два стиля оформления ссылок:

* Гиперссылка, с немедленным указанием адреса (внутритекстовая);

* Гиперссылка, подобная сноске.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

    [пример](http://example.com/ "Необязательная подсказка")

При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).

    [пример][id]:

Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок:

    [пример] [id]: 

В этом случае возможно определить идентификатор в любом месте документа:

    [id]: http://example.com/ "Необязательная подсказка"

В результате на экран выводится следующее: [пример] [id] [id]: http://example.com/ "Необязательная подсказка" Иными словами, она состоит из следующих элементов:

Идентификатор ссылки, окружённый квадратными скобками (которым может предшествовать необязательный отступ от одного до трёх пробелов);
* Двоеточие;
* Один или несколько пробелов (или символов табуляции);
* URL гиперссылки;
* Необязательный заголовок (подсказка к изображению, которая всплывает при наведении на него) гиперссылки, заключённый либо в двойные или одиночные кавычки, либо в скобки.

Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:

    [текст ссылки][a]
    [текст ссылки][A]

Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется и в качестве её имени, а вторая пара квадратных скобок остаётся пустою. Например, чтобы сделать слово «Example» гиперссылкой, ведущей на сайт http://example.com/, достаточно написать:

    [Example][]

и затем определить гиперссылку:

    [Example]: http://example.com/

В результате на экран выводится следующее: [Example][] [Example]: http://example.com/


## **Кодовые фрагменты строк**

Чтобы отметить фрагмент строки, содержащий код, необходимо окружить его обратными апострофами «`». При использовании кодовых фрагментов строк текст будет отображаться в виде моноширинного шрифта. В отличие от блоков кода, кодовый фрагмент позволяет поместить код внутрь обычного абзаца текста. Кодовый фрагмент строки в языке Markdown выглядит следующим образом:

Используйте оператор `if` (кнопка под esс, где русская Ё, на англ раскладке)

## **Изображения**

В Markdown существует 2 способа вставки изображений в документ:

a. С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

    ![Альтернативный текст](/путь/к/изображению.jpg)

или

    ![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")

Иными словами, он состоит из следующих элементов:

* восклицательный знак;
* квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
* круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.

b. С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:

    ![Альтернативный текст][id]


где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

    [id]: путь/к/изображению "Необязательная подсказка"

Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).

## **Дополнительные элементы**

### **Обратный слеш**

Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении. Полный список данных символов приводится ниже:

«\» - слеш;

«`» - обратный апостроф;

«*» - звездочка;

«_» - символ подчеркивания;

«{}» - фигурные скобки;

«[]» - квадратные скобки;

«()» - круглые скобки;

«#» - символ решетки;

«+» - плюс;

«-» - минус (дефис);

«.» – точка;

«!» - восклицательный знак.

## **Автоматические ссылки**

Markdown поддерживает упрощённый порядок автоматического создания ссылок для URL-адресов и адресов электронной почты. Для этого достаточно поместить URL-адрес или почтовый адрес в угловые скобки, и Markdown сделает его гиперссылкой. В отличие от вышеописанных стилей, в данном случае сам же URL-адрес или почтовый адрес становится и текстом гиперссылки. Автоматические ссылки на адреса электронной почты работают аналогично. Автоматические ссылки в языке Markdown выглядят следующим образом

    <http://example.com/>

В результате на экран выводится следующее: http://example.com/

Автоматическая ссылка на адрес электронной почты в Markdown выглядит следующим образом

    <address@example.com>

В результате на экран выводится следующее: address@example.com

## **Специальные символы HTML**

В языке HTML существует два символа, требующих специального рассмотрения: это символы («<») и («&»). Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения специального символа HTML. Для того чтобы использовать эти символы в их буквальном смысле, необходимо заменить их элементами HTML, а именно &lt; и &amp; соответственно. При использовании Markdown подобных действий совершать не нужно. Он позволяет использовать эти символы в исходном виде. В случае если амперсанд используется как часть спецсимвола HTML, он останется неизменным. В противном случае Markdown преобразует его в &amp;.



