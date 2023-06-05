# Base rules

Ну это база, без этого никуда.

## Tools

### :information_source: ch-base-info-try-phind

[Phind][phind] — поисковый движок с [AI][ai] для разработчиков.

Начал пользоваться только недавно, поэтому в разделе _Info_.
Но уже оч нравится.

## Search

### :warning: ch-base-warning-google-it-in-english

Ищи в интернете на английском языке.

Переходи к поиску на русском только после
10 прочитанных ресурсов на английском.

!!! failure "Не надо так"

    _Основано на реальном диалоге_

    ```mermaid
    sequenceDiagram
        %%{init: { "mirrorActors": false } }%%
        participant you
        participant chaberch
        chaberch->>you: Какое приложение будем использовать <br/> для работы с openapi?
        you->>chaberch: Swagger. Он умеет то-то и то-то.
        chaberch->>you: Только он так умеет?
        you->>chaberch: Я других не нашел.
        chaberch->>you: Как искал?
        you->>chaberch: "графические средства для работы с openapi", <br/> смотрел первые 7-10 ссылок.
        Note over chaberch: Гуглит "openapi ui tools"
        Note over chaberch: По первой же ссылке <br/> сотня приложений <br/> для работы с openapi
    ```

### :no_entry: ch-base-error-dont-use-yandex

Не используй Яндекс для поиска англоязычных статей.

### :no_entry: ch-base-error-dont-auto-translate

Не используй автоматический перевод страницы.

Переводи английский текст самостоятельно.
Используй [гугл-переводчик][google-translate] для незнакомых слов,
и [Reverso][reverso] для незнакомых словосочетаний.

## Teamwork

### :no_entry: ch-base-error-i-dont-know

Не притворяйся, что знаешь то, чего на самом деле не знаешь.

!!! failure "Плохо"

    _Основано на реальном диалоге_

    ```mermaid
    sequenceDiagram
        %%{init: { "mirrorActors": false } }%%
        participant you
        participant chaberch
        chaberch->>you: Ты знаешь что такое REST?
        you->>chaberch: Да!
        chaberch->>you: Что такое REST?
        you->>chaberch: Ну… это… э… что-то типа как HTTP…
    ```

!!! success "Хорошо"

    ```mermaid
    sequenceDiagram
        %%{init: { "mirrorActors": false } }%%
        participant you
        participant chaberch
        chaberch->>you: Ты знаешь что такое REST?
        you->>chaberch: Нет, но если это требуется для решения задачи,<br/> то изучу в ближайшее время.
        Note over you: Уходит изучать REST
    ```

### :no_entry: ch-base-error-learn-how-to

Изучи как работать с инструментом перед тем как применять его.

!!! failure "Не надо так"

    _Основано на реальном диалоге_

    ```mermaid
    sequenceDiagram
        %%{init: { "mirrorActors": false } }%%
        participant you
        participant chaberch
        Note over you: Пишет кривой нерабочий код<br/> на асинхронных функциях
        you-->>chaberch: Скидывает код на ревью
        chaberch->>you: Ты не понимаешь что делаешь,<br/> читай про асинхронные функции
        you->>chaberch: "изучать всё" - как по мне напрасная трата времени,<br/> потому что я считаю, что понимаю что тут происходит
    ```

### :no_entry: ch-base-error-obscurity

Не создавай неизвестность.
Даже отрицательный результат лучше неизвестности.

!!! failure "Не надо так"

    _Основано на реальном диалоге_

    ```mermaid
    sequenceDiagram
        %%{init: { "mirrorActors": false } }%%
        participant you
        participant chaberch
        chaberch->>you: Вот задание.<br/> До конца этой недели доложи о результатах
        you->>chaberch: Хорошо
        Note over you: Пропал на 3 недели
        chaberch->>you: Почему не доложил?
        you->>chaberch: Мне было неловко писать,<br/> потому что видимых результатов практической части не было<br/> и не хотелось сообщать об отсутствии результатов.<br/> А потом было неловко из-за пропущенных сроков
    ```

[phind]: https://www.phind.com/
[ai]: https://ru.wikipedia.org/wiki/%D0%98%D1%81%D0%BA%D1%83%D1%81%D1%81%D1%82%D0%B2%D0%B5%D0%BD%D0%BD%D1%8B%D0%B9_%D0%B8%D0%BD%D1%82%D0%B5%D0%BB%D0%BB%D0%B5%D0%BA%D1%82
[google-translate]: http://translate.google.ru/
[reverso]: https://context.reverso.net/%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D0%BE%D0%B4/
