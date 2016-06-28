# Что такое Кодревью?
Кодревью — систематическая проверка исходного кода с целью обнаружения и исправления ошибок, которые остались незамеченными в начальной фазе разработки. 

## Основные цели проведения кодревью:
- Найти и справить дефекты ПО на ранней стадии.
- Улучшить коллективное и индивидуальное знание проекта.
- Поддерживать выбранный уровень однообразности, дизайна и стиля.
- Найти и разобрать ошибки, особенности проекта, интересные подходы и задачи - таким образом повысив профессиональный уровень команды.
- Снизить зависимость команды от конкретного разработчика, улучшить коллективное владение кодом.
- Другая перспектива ревьювера позволяет найти больше подходов к решению проблемы. Объективная критика помогает понять заблуждения разработчика.

## Основные аспекты разработки ПО, которые затрагивает кодревью:
* Тесты
* Кодстаил и комментарии
* Обработка ошибок
* Утечки ресурсов
* Потокобезопасность
* Дизайн классов
* Производительность
* Соответствие функциональным требованиям
* Безопасность

Как и любой навык, навык проведения кодревью совершенствуется при практике. Ниже представлены несколько общих советов для разработчика и ревьювера:

## Советы для разработчика
* Главным и самый первым ревьювером является сам разработчик.
* Создай себе чеклист, на котором будут основные проверки, проводимые ревьюверами.Это поможет избежать банальных и глупых багов, таких как: Отсутствие прав, неправильная кодировка файла, несобирающийся проект и тому подобное. Будет очень обидно сдать задачу на проверку, которую ревьювер завернет обратно через 5 минут.
* Дистанцируй себя от своего кода. Основная задача ревью - найти баги, а кто ищет - тот находит. Не принимай найденные баги близко к сердцу - скорее всего в твоем коде есть баг, а то и несколько.
* Научись у ревьювера чему-то новому. Если ревьювер предлагает простое и элегантное решение проблемы, то это win-win - Ты научишся чему то и плохой код не попадет в продакшн.
* Не переписывай код без повода. Не всегда ревьювер будет предлагать адекватные решения. Если считаешь, что ревьювер не прав - обьективно аргументируй.
* Не закрывайся в себе. Если тебе что-то не понятно, задай ревьюверу вопрос. Вынеси проблему на общее обсуждение. От этого никто не пострадает, зато все будут все понимать.
* Поддерживай стандарты кодирования. Про стандарты кодирования сказано многое, и если уж все под ними подписались, то необходимо их поддерживать.

## Советы для ревьювера
* Просматривай 200-400 строк кода за раз, после сделай перерыв.
* Критикуй код, а не разработчика. Цель твоего комментария - сделать так, чтобы разработчик написал хороший код. Указание и анализ ошибки в позитивном ключе помогают достигнуть цели. Комментарии в негативном ключе без внятных аргументов - нет.
* Реальный авторитет идет от знаний, а не от должности или формального положения. Знание увеличивает авторитет и уважение среди других разработчиков. Кодревью - хороший способ продемонстрировать свои знания.
* Задавай вопросы прежде чем делать утверждения. Как правило ревьювер не настолько владеет контекстом, как разработчик. Возможно для того, что кажется неправильным есть своя причина.
* Не забудь пояснить. Одна из целей кодревью - прокачать навыки разработчика. Если ты знаешь, что так будет лучше, поясни, почему.
* Часто есть несколько способов сделать одно и то же. Если подход, который кажется тебе необычным позволяет эффективно достичь цели, то почему бы и нет? 

## Чеклист для проверки С# кода
1. Убедись, что проект собирается без предупреждений и ошибок.
2. Проведи анализ кода - цикломатическая сложность методов не должна превышать 20. Тестовое покрытие должно быть не мение 70%.
3. Удали неиспольлзуемые директивы using и недостижимый код.
4. Убедись, что везде, где необходимо есть проверки на null.
5. Если код в нескольких методах повторяется - вынеси его в отдельный метод.
6. Проверь, что все неуправляемые ресурсы корректно освобождаются.
7. Убедись, что во всех необходимых местах используется обработка исключений и логирование, если оно необходимо.
8. Используй анонимные типы, если тип будет использоваться только 1 раз.
9. Проверь уровни доступа разработаных классов, методов и полей.
10. Запусти тесты, проверь что они проходят за адекватное время.


Источники:
https://blog.codinghorror.com/the-ten-commandments-of-egoless-programming/
http://www.developer.com/java/other/article.php/3579756
http://www.techrepublic.com/article/developers-guide-to-peer-reviews/1050834/
https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/
http://www.codeproject.com/Articles/593751/Code-Review-Checklist-and-Guidelines-for-Csharp-De
