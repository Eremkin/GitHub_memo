 [< к содержанию](./readme.md)
 # Синтаксис Markdown (краткая шпаргалка)

 Markdown - облегченный язык разметки. Для его использования не требуется долгого обучения. Использование Markdown значительно ускоряет разработку, и документирование, в частности на GitHub. 

 Стоит отметить, что материал составлен для *дополненного и улучшенного варианта* языка Markdown — **Github Flavoured Markdown**, сокращенно GFM

 Ниже приведен основной синтаксис языка, требуемый для полноценного составления документов на GitHub

 ## 1. Заголовки
 ---

 Для написания заголовков в Markdown используют знак # (хэш). Если необходимо несколько уровней заголовков, h1 - h6, нужно изменить количество хэшей (#) перед текстом заголовка.

код:
```
# Заголовок h1
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6
```

Результат: 
# Заголовок h1
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6


## Списки
---


Для разметки **неупорядоченных списков** можно использовать или `*`, или `-`, или `+`:

*Код:*
```
- элемент 1
- элемент 2
- элемент ...
```
*Результат:*
- элемент 1
- элемент 2
- элемент ...

**Вложенные пункты** создаются 4-мя пробелами перед маркером пункта:

*Код:*
```
* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...
```
*Результат:*

* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...

**Упорядоченный список:**

*Код:*
```
1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
4. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.
```

*Результат:*
1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
4. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

*На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. Можно сделать и так:*
*Код:*
```
0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4
```
*Результат:*
1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
4. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

**Список с абзацами:**

*Код:*
```
* Раз абзац. Lorem ipsum dolor sit amet, consectetur adipisicing elit.

* Два абзац. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

* Три абзац. Ea, quis, alias nobis porro quos laborum minus sed fuga odio dolore natus quas cum enim necessitatibus magni provident non saepe sequi?

    Четыре абзац (Четыре пробела в начале или один tab).
```
*Результат:*

* Раз абзац. Lorem ipsum dolor sit amet, consectetur adipisicing elit.

* Два абзац. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

* Три абзац. Ea, quis, alias nobis porro quos laborum minus sed fuga odio dolore natus quas cum enim necessitatibus magni provident non saepe sequi?

    Четыре абзац (Четыре пробела в начале или один tab).
    


## Цитаты


Цитаты оформляются как в емейлах, с помощью символа `>`.

*Код:*
```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
```

*Результат:* 
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.


Или более ленивым способом, когда знак `>` ставится перед каждым элементом цитаты, будь то абзац, заголовок или пустая строка:
```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
```
Результат тот-же ))

**В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:**

*Код:*
```
> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");
```
Результат: 
## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");




Синтаксис вставки кода!



При подготовке материала использованы источники: 
https://paulradzkov.com/2014/markdown_cheatsheet/
https://daringfireball.net/projects/markdown/syntax

