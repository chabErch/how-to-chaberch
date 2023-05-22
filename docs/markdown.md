# Markdown rules

I :heart: markdown

## Info

### ch-md-info-try-typora

[Typora][typora] —
самый классный и минималистичный [WYSIWYG][wysiwyg] редактор для markdown,
в нем прям **хочется** писать текст.
Не бесплатный.
Если есть возможность купить его, то сделай это, не пожалеешь.

### ch-md-info-try-marktext

[MarkText][marktext] —
один из лучших бесплатных [WYSIWYG][wysiwyg] редакторов под markdown.
Но есть опасения, что разработчики его забросили —
последние обновления были около года назад.

### ch-md-info-use-vs-code

Плагины в [VS Code][vs-code] помогут контролировать содержимое документа:

- [markdownlint][markdownlint] —
  линтер для markdown

- [Russian - Code Spell Checker][russian-code-spell-checker] —
  проверка русской орфографии

Ну и [настрой направляющие][vs-code-rulers].

## Warning

### ch-md-warning-file-name-case

Именуй markdown документы согласно [kebab-case][kebab-case].

!!! failure "Плохо"

    `My document.md`

!!! success "Хорошо"

    `my-document.md`

### ch-md-warning-code-blocks-style

Используй апострофы (`` ``` ``) для обозначения блока с кодом.

!!! failure "Плохо"

    ```markdown
    ~~~python
    print("Hello")
    ~~~
    ```

    ```markdown
        print("Hello")
    ```

!!! success "Хорошо"

    ~~~markdown
    ```python
    print("Hello")
    ```
    ~~~

### ch-md-warning-emphasis-punctuation

Знаки препинания не включаются
в блоки с жирным текстом, курсивом и подчеркиванием.

!!! failure "Плохо"

    ```markdown
    Откройте окно _Пользователи системы._
    ```

!!! success "Хорошо"

    ```markdown
    Откройте окно _Пользователи системы_.
    ```

### ch-md-warning-image-file-name-case

Именуй изображения для документов согласно [kebab-case][kebab-case].

!!! failure "Плохо"

    ```markdown
    ![Милый котенок](my-document.assets/CuteKitten.png)
    ```

!!! success "Хорошо"

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.png)
    ```

### ch-md-warning-image-base-format

Используй формат `png` для растровых картинок без анимации.

!!! failure "Плохо"

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.jpg)
    ```

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.gif)
    ```

!!! success "Хорошо"

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.png)
    ```

## Error

### ch-md-error-first-line-h1

Первой строкой в документе должен идти заголовок первого уровня.

!!! failure "Плохо"

    ```markdown
    Это документ без заголовка
    
    ```
    
    ```markdown
    ## Заголовок документа
    
    ```

!!! success "Хорошо"

    ```markdown
    # Заголовок документа
    
    ```

### ch-md-error-heading-style

Используй [ATX-Style][atx-style-headers] для обозначения заголовков.

!!! failure "Плохо"

    ```markdown
    Заголовок документа
    ===================
    
    Следующий заголовок
    -------------------
    
    ```

!!! success "Хорошо"

    ```markdown
    # Заголовок документа
    
    ## Следующий заголовок
    
    ```

### ch-md-error-trailing-punctuation-in-heading

В конце заголовков знаки препинания не ставятся.

!!! failure "Плохо"

    ```markdown
    # Заголовок документа.
    ```

!!! success "Хорошо"

    ```markdown
    # Заголовок документа
    ```

### ch-md-error-increment-heading-levels

Каждый следующий уровень заголовка может быть не больше чем на единицу от предыдущего.

!!! failure "Плохо"

    ```markdown
    # Заголовок документа
    
    ### Следующий заголовок
    
    ```

!!! success "Хорошо"

    ```markdown
    # Заголовок документа
    
    ## Следующий заголовок
    
    ```

### ch-md-error-separate-blocks

Отделяй блоки одной пустой строкой.

!!! failure "Плохо"

    ```markdown
    # Заголовок документа
    Текст документа.
    ```

    ```markdown
    # Заголовок документа


    Текст документа.
    ```

!!! success "Хорошо"

    ```markdown
    # Заголовок документа
    
    Текст документа.
    ```

### ch-md-error-line-length

В заголовках, списках, блоках с текстом и в блоках кода
должно быть не больше 80 символов в каждой строке.

Переносы делать в местах логических пауз.

!!! failure "Плохо"

    ```markdown
    В мультиселекторе пользователь выбирает всех сотрудников, которые сдали свои предпочтения.
    ```

!!! success "Хорошо"

    ```markdown
    В мультиселекторе пользователь выбирает всех сотрудников,
    которые сдали свои предпочтения.
    ```

### ch-md-error-new-line-sentence

Каждое предложение должно начинаться с новой строки.

!!! failure "Плохо"

    ```markdown
    Черта является верхней границей объявления,
    расположенного на доске объявлений. Но при просмотре объявления,
    выше черты отображается поле с более подробной информацией об ...
    ```

!!! success "Хорошо"

    ```markdown
    Черта является верхней границей объявления,
    расположенного на доске объявлений.
    Но при просмотре объявления,
    выше черты отображается поле с более подробной информацией об ...
    ```

### ch-md-error-italic-style

Используй `_` для выделения курсивом.

!!! failure "Плохо"

    ```markdown
    Откройте окно *Пользователи системы*.
    ```

!!! success "Хорошо"

    ```markdown
    Откройте окно _Пользователи системы_.
    ```

### ch-md-error-bold-style

Используй `**` для выделения жирным.

!!! failure "Плохо"

    ```markdown
    __Архив__ — это каталог, который содержит ...
    ```

!!! success "Хорошо"

    ```markdown
    **Архив** — это каталог, который содержит ...
    ```

### ch-md-error-emphasis-instead-of-a-heading

Не используй текст выделенный жирным, курсивом или подчеркиванием
в качестве заголовка.

!!! failure "Плохо"

    ```markdown
    **Параметры объекта**

    1. `name` — название объекта;
    ```

### ch-md-error-ul-style

Используй `-` для обозначения неупорядоченных списков на всех уровнях.

!!! failure "Плохо"

    ```markdown
    * первый элемент
    * второй элемент
        + дочерний элемент
    ```

!!! success "Хорошо"

    ```markdown
    - первый элемент
    - второй элемент
        - дочерний элемент
    ```

### ch-md-error-ul-indentation

Используй 4 пробела на уровень для вложенных неупорядоченных списков.

!!! failure "Плохо"

    ```markdown
    - первый элемент
    - второй элемент
      - дочерний элемент
    ```

!!! success "Хорошо"

    ```markdown
    - первый элемент
    - второй элемент
        - дочерний элемент
    ```

### ch-md-error-bare-url

Пользователь не должен видеть голых url,
если только этот url не является вопросом обсуждения.

!!! failure "Плохо"

    ```markdown
    Для поиска в интернете надо перейти на сайт 
    https://www.google.com.
    ```

    ```markdown
    Для поиска в интернете надо перейти на сайт
    <https://www.google.com>.
    ```

!!! success "Сойдет"

    ```markdown
    Для поиска в интернете надо перейти на сайт
    [Google](https://www.google.com).
    ```

!!! success "Отлично"

    ```markdown
    Для поиска в интернете надо перейти на сайт [Google][google].
    
    [google]: https://www.google.com
    ```

### ch-md-error-new-line-url

Переноси ссылки на новую строку, если они определены сразу.

!!! failure "Плохо"

    ```markdown
    Искать надо через [Google](https://www.google.com), и только так.
    ```

!!! success "Хорошо"

    ```markdown
    Искать надо через
    [Google](https://www.google.com),
    и только так.
    ```

### ch-md-error-code-blocks-language

Указывай язык для блоков с кодом.

!!! failure "Плохо"

    ~~~markdown
    ```
    print("Hello")
    ```
    ~~~

!!! success "Хорошо"

    ~~~markdown
    ```python
    print("Hello")
    ```
    ~~~

### ch-md-error-image-alt-text

Добавляй описание к изображениям.

!!! failure "Плохо"

    ```markdown
    ![](my-document.assets/cute-kitten.png)
    ```

!!! success "Хорошо"

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.png)
    ```

### ch-md-error-image-location

Храни изображения для документа в папке с названием `<document_name>.assets`,
где `<document_name>` — название документа.

Папка должна располагаться по тому же пути, что и сам документ.

!!! failure "Плохо"

    ```markdown
    ![Милый котенок](C:/Images/cute-kitten.png)
    ```

    ```markdown
    ![Милый котенок](./cute-kitten.png)
    ```

!!! success "Хорошо"

    ```markdown
    ![Милый котенок](my-document.assets/cute-kitten.png)
    ```

### ch-md-error-eof

Документ должен заканчиваться пустой строкой.

[typora]: https://typora.io/
[wysiwyg]: https://ru.wikipedia.org/wiki/WYSIWYG
[marktext]: https://github.com/marktext/marktext
[vs-code]: https://code.visualstudio.com/
[markdownlint]: https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint
[russian-code-spell-checker]: https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-russian
[vs-code-rulers]: https://levelup.gitconnected.com/do-you-know-about-rulers-in-visual-studio-code-f754b221a135
[kebab-case]: https://medium.com/@vladimirmorulus/%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D0%B0-%D0%BF%D0%BE-case-camelcase-kebab-case-pascalcase-snake-case-%D0%B8-%D0%B2%D1%81%D0%B5-case-ecda10463fa8#0104
[atx-style-headers]: https://riptutorial.com/markdown/example/2217/atx-style-headers
