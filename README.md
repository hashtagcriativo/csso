# Использование

Пока наиболее удобно так:

* git clone git@github.com:afelix/csso.git
* открыть в браузере файл csso.html
* проверять

Неудобно:

* git clone git@github.com:afelix/csso.git
* node ccli.js файл.css
* в ccli.js раскомментировать нужный формат вывода и комментировать ненужный

# Done

### Мелкое

* убирает лишние whitespace;
* убирает комментарии;
* убирает лишние ';';
* убирает неправильный @charset;
* убирает пустые блоки;
* оптимизирует цвет;
* оптимизирует числа;
* склеивает multiline строки;
* font-weight normal и bold => 400 и 700;
* не трогает expression.

### Крупное

* убирает всё, что не попадает в computed stylesheet;
* группирует selector и property в структуры с наименьшей длиной в символах;
* порядок, в котором следуют оригинальные selector и property, сохраняется.

# TODO

### Мелкое

* более удобный command-line;
* не "оптимизировать", если результат больше оригинала (такое бывает, если большой CSS после csso снова отправить в csso);
* оптимизация внутри @font-face;
* документировать код.

### Крупное

* оптимизация shorthand;
* позволять комментариями исключать property (и блоки?) из обработки;
* невалидный CSS;
* мануал.
