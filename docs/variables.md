# Variables rules

> в программировании есть только две сложные вещи:
> инвалидация кеша, выбор имени переменной, и ошибки на единицу.

## Boolean

### :warning: ch-var-warning-bool-part-of-speech

Название для булевой переменной должно быть общим вопросом
(ответом на общий вопрос может быть либо _да_, либо _нет_).

Используй в названиях такие частицы как _is_, _has_, _was_ и т.д.

!!! failure "Плохо"

    === "Python"

        ```py
        # Открыто то ли модальное окно
        open = False

        # Есть ли у пользователя доступ
        access = False
        ```

    === "Js"

        ```js
        // Открыто то ли модальное окно
        const open = false

        // Есть ли у пользователя доступ
        const access = false
        ```

!!! success "Хорошо"

    === "Python"

        ```py
        # Открыто то ли модальное окно
        is_open = False

        # Есть ли у пользователя доступ
        has_access = False
        ```

    === "Js"

        ```js
        // Открыто то ли модальное окно
        const isOpen = false

        // Есть ли у пользователя доступ
        const hasAccess = false
        ```
