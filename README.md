# Gulp-hm-includer


### Configuration

- `<pattern>` - объект с маской заменяемого вхождения или название маски из библиотеки patterns
    - `<expr>` - регулярное выражение или строка замены
    - `<path>` - маска пути в expr. Или номер маски '$n'
    - `<wrap>` - обёртка для вставляемых данных. например
        
        `pattern.wrap = "<style>\n    {{}}\n<style>"`

<br>
<br>


> ВНИМАНИЕ!!!<br>
> Используя плагин в разных пайпах, вы рискуете не получить желаемого результата.
> 1. Cодержащиеся в подключаемых файлах относительные ссылки могут не действовать в текущем документе.
>
> 2. Также, будет важен порядок пайпов с плагином. Потому как в подключенном файле могут содержаться ссылки попадающие под шаблон предыдущих пайпов.

