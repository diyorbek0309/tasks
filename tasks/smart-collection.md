# smart-collection

**smart-collection** - коллекция элементов с возможностями сортировки, поиска, фильтрации по нескольким фильтрам, добавления/удаления элементов в избранное, а также с интерактивной страницей избранного.  

## Ключевые навыки:
- TypeScript
- OOP
- создание SPA
- сортировка данных
- реализация поиска
- фильтрация данных
- сбор и систематизация данных
- работа с асинхронными запросами
- генерирование html при помощи TypeScript

<kbd>![screenshot](images/smart-collection.png)</kbd>

- [Демо работы прототипа приложения](https://react-course-comfy-sloth-store.netlify.app/products)  
*Если описание задания не совпадает с прототипом, задание выполняется согласно описанию*

## Подготовительный этап работы над проектом
- выберите тематику коллекции. Это может быть:
  - коллекция книг/картин/почтовых марок
  - коллекция фильмов/сериалов/мультфильмов
  - коллекция растений/животных/цветов
  - коллекция стран, в которых вы хотели бы побывать/достопримечательностей, которые хотели бы посмотреть
  - коллекция ёлочных украшений и/или новогодних подарков
  - или любая другая тематика на ваш выбор
- создайте JSON-файл в котором опишите элементы коллекции. Всего в коллекцию необходимо добавить не меньше 15 элементов. Для каждого из них укажите название, небольшое описание (2-3 предложения), ссылку на изображение, и не меньше 5 различных характеристик, которые понадобятся для сортировки и фильтрации
- исходя из выбранной вами тематики коллекции, определите функционал страницы избранного. На странице избранного отображаются все выбранные элементы коллекции и обеспечивается возможность интерактивного взаимодействия с ними:
  - для коллекции мебели это может быть комната/квартира, которую можно обставить выбранной мебелью, с возможностью перемещения и поворота элементов мебели, выбора их модификации по цвету или оформлению
  - для коллекции книг это может быть книжная полка с возможностью поставить/убрать/повернуть/листать книгу, прочитать её название и автора
  - для коллекции ёлочных украшений это может быть ёлка, на которую можно перетащить (повесить) выбранные украшения. После того, как ёлка украшена, ёлочная гирлянда мерцает, шары покачиваются и звенят при наведении
  - для коллекции аквариумных рыбок это может быть аквариум, в который можно поместить выбранных рыбок, и в котором они будут плавать
  - страны, в которых планируете побывать, можно разместить на карте, при наведении на страну отображается расстояние до неё и т.д. 

## Структура приложения
Приложение состоит из трёх страниц
- главная страница коллекции
- страница элемента коллекции
- страница избранного

## Функционал приложения
1. Главная страница коллекции содержит карточки всех элементов коллекции. Также на главной странице коллекции размещаются фильтры, строка поиска, поле для сортировки. С главной страницы коллекции можно перейти на страницу избранного. Выполняются требования к вёрстке +10
2. Карточки с элементами коллекции на главной странице могут отображаться в виде таблицы и в виде  списка как в [прототипе приложения](https://react-course-comfy-sloth-store.netlify.app/products) +25
   - в виде таблицы карточки с элементами коллекции содержат изображение элемента коллекции, его название и одну ключевую характеристику, например, цену +10
   - в виде списка карточки с элементами коллекции содержат изображение элемента коллекции, его название, одну ключевую характеристику, например, цену и короткое описание +10
   - есть возможность переключения отображения карточек с элементами коллекции в виде таблицы и в виде  списка. При клике по карточке или кнопке на ней происходит переход на страницу элемента коллекции. +5
3. Сортировка +25
   - сортировка карточек с элементами коллекции по названию в возрастающем и спадающем порядке +10
   - сортировка карточек с элементами коллекции по их ключевой характеристике в возрастающем и спадающем порядке +10
   - в процессе сортировки карточки с элементами коллекции плавно меняют своё положение с эффектами анимации [Демо](https://codepen.io/Vestride/pen/ZVWmMX). Для плавного изменения положения карточек на странице может использоваться js-библиотека +5
4. Фильтры +25
   - не меньше пяти фильтров, по которым можно фильтровать карточки с элементами коллекции +10
   - фильтры уникальные по внешнему виду и оформлению, примеры уникальных фильтров есть в [прототипе приложения](https://react-course-comfy-sloth-store.netlify.app/products) - два балла за каждый уникальный фильтр, но не больше 10 баллов +10
   - в процессе фильтрации карточки с элементами коллекции плавно меняют своё положение с эффектами анимации [Демо1](https://codepen.io/Vestride/pen/ZVWmMX), [Демо2](https://codepen.io/ComeonCreative/pen/WxwPaW). Для плавного изменения положения карточек на странице может использоваться js-библиотека +5
5. Поиск +25
   - при открытии приложения курсор находится в поле поиска +2
   - автозаполнение поля ввода поискового запроса отключено (нет выпадающего списка с предыдущими запросами) +2
   - есть placeholder +2
   - в поле поиска есть крестик, позволяющий очистить поле поиска +2
   - если нет совпадения последовательности букв в поисковом запросе с названием элемента коллекции, выводится уведомление о том, что совпадение не обнаружено, например "Sorry, no products matched your search" +2 
   - при вводе поискового запроса под строкой поиска появляется выпадающее окно, в котором по мере ввода отображаются названия тех элементов коллекции, в которых есть указанные в поиске буквы в указанном порядке. При этом не обязательно, чтобы буквы были в начале слова +5
   - при вводе поискового запроса можно выбрать элемент коллекции кликом по его названию в выпадающем окне под строкой поиска. При этом выпадающее окно исчезает, на странице остаётся только выбранный элемент +5
   - при вводе поискового запроса при нажатии клавиши `Enter` выпадающее окно под строкой поиска исчезает, на странице остаются только те элементы коллекции, в которых есть указанные в поиске буквы в указанном порядке. При этом не обязательно, чтобы буквы были в начале слова +5
6. Страница элемента коллекции содержит его изображение, название, описание, все характеристики. Со страницы элемента коллекции можно перейти на главную страницу коллекции и на страницу избранного. Выполняются требования к вёрстке +10
7. На главной странице коллекции и на странице элемента коллекции есть возможность добавить элемент в избранное +10
8. На странице элемента коллекции при наведении курсора на разные части изображения они отображаются в увеличенном виде. [Демо](https://output.jsbin.com/kerili/1). Отличие от демо: 1) нет круглой границы области увеличения, увеличенная часть занимает всё изображение 2) границы изображения остаются неизменными. Когда курсор отвести от изображения, оно возвращается к первоначальному виду +10
9. Страница избранного содержит карточки всех выбранных пользователем элементов коллекции. Со страницы избранного можно перейти на главную страницу коллекции. Выполняются требования к вёрстке +10
10. На странице избранного возле каждой карточки с элементом коллекции указывается количество выбранных элементов и есть возможность изменить их количество в пределах от 0 до 10. Если пользователь уменьшил количество элементов до 0, изображение элемента становится черно-белым +10
11. На странице избранного есть интерактивное демо на котором отображаются выбранные пользователем элементы коллекции, или их можно туда перетаскивать +10
12. Есть возможность взаимодействия пользователя с интерактивным демо и его элементами - 10 баллов за каждую сложную, уместную, качественно реализованную функциональность, но не больше 30 баллов +30
13. Высокое качество оформления приложения, дополнительные, не указанные в задании, сложные, интересные, уместные анимации, другие сложно реализуемые и качественно выполненные элементы оформления +10
14. Дополнительный, не указанный в задании, сложный в реализации функционал, улучшающий качество приложения и удобство пользования им +10

## Критерии оценки cross-check
**Максимальный балл за задание +200**

Для удобства проверки выведите в консоль браузера самооценку своего проекта по пунктам с указанием баллов за каждый выполненный вами пункт.

Баллы за отдельные пункты требований указаны в разделе ["Структура и функционал приложения"](#функционал-приложения)

Разница между максимальной оценкой за приложение (200 баллов) и максимально возможным количеством баллов за выполнение всех пунктов требований (220 баллов) позволит сгладить возможные ошибки проверяющих в ходе кросс-чека, неточности в описании задания, разное понимание требований задания проверяющим и проверяемым.

## Проверка задания ментором
**Максимальный балл за задание +200**

1. Репозиторий +20
   - pull request выполнен в соответствии с [требованиями](https://docs.rs.school/#/pull-request-review-process?id=Требования-к-pull-request-pr) +10
   - ведётся история коммитов, названия коммитов даются согласно [гайдлайну](https://docs.rs.school/#/git-convention) +10
2. Технические требования +90
   - для написания кода приложения используется TypeScript +50
   - код разбит на модули +10
   - для сборки кода используется webpack +10
   - используется eslint с конфигурацией eslint-config-airbnb-base, ошибки линтера исправлены, в eslint не добавляются собственные правила без согласования с ментором +10
   - в качестве источника данных создан и используется JSON-файл +10  
3. Качество кода +60
   - правильное наименование переменных и функций +10
   - используется prettier, код отформатирован, хорошо читается +10
   - нет дублирования кода, повторяющиеся фрагменты кода вынесены в функции, оптимальный размер функций, выполняется рекомендация: одна функция – одна задача +10
   - нет глубокой вложенности циклов, нет магических чисел +10
   - используются фичи ES6 и выше: let, const для объявления переменных, стрелочные функции, Spread/Rest операторы, деструктуризация, классы, async/await и т.д +10
   - у ментора нет замечаний к качеству кода, либо все замечания ментора исправлены +10
4. Оформление и функционал приложения +30
   - у ментора нет замечаний к оформлению и функционалу приложения, либо все замечания ментора исправлены +30

## Требования к репозиторию
- задание выполняется в **приватном репозитории школы** [Как работать с приватным репозиторием](https://docs.rs.school/#/private-repository?id=Как-работать-с-приватным-репозиторием)
- в приватном репозитории школы от ветки `main` создайте ветку с названием задания, в ней создайте папку с названием задания, в папке разместите файлы проекта
- для деплоя используйте gh-pages [Как сделать деплой задания из приватного репозитория школы](https://docs.rs.school/#/private-repository?id=Как-сделать-деплой-задания-из-приватного-репозитория-школы)
- при невозможности использовать gh-pages, используйте для деплоя https://app.netlify.com/drop. Название страницы дайте по схеме: имя гитхаб аккаунта - название таска
- история коммитов должна отображать процесс разработки приложения. [Требования к коммитам](https://docs.rs.school/#/git-convention?id=Требования-к-именам-коммитов)
- после окончания разработки необходимо сделать Pull Request из ветки приложения в ветку `main` [Требования к Pull Request](https://docs.rs.school/#/pull-request-review-process?id=Требования-к-pull-request-pr). **Мержить Pull Request из ветки разработки в ветку `main` не нужно**

## Технические требования
- для написания кода приложения используйте TypeScript
- разбейте код на модули
- для сборки кода используйте webpack
- в качестве источника данных создайте и используйте JSON-файл
- используйте eslint с конфигурацией eslint-config-airbnb-base
- работа приложения проверяется в браузере Google Chrome последней версии
- можно использовать [bootstrap](https://getbootstrap.com/), [material design](https://material.io/), css-фреймворки, html и css препроцессоры
- не разрешается использовать jQuery, другие js-библиотеки и фреймворки, за исключением библиотек, обеспечивающих анимацию перемещения элементов на странице
- использование Angular/React/Vue допускается только по согласованию с ментором

## Рекомендации по написанию кода
- основное и самое важное требование к коду - его работоспособность: работающий код лучше идеального, но не работающего
- тем не менее, есть те рекомендации, которым необходимо следовать даже начинающему разработчику:
  - правильное наименование переменных и функций
  - используйте prettier для форматирования кода, отформатированный код проще читается
  - избегайте дублирования кода, повторяющиеся фрагменты кода вынесите в функции
  - стремитесь к оптимальному размеру функций, следуйте правилу: одна функция – одна задача
  - избегайте глубокой вложенности циклов, магических чисел
  - используйте фичи ES6 и выше, например, let, const для объявления переменных, стрелочные функции и т.д

## Требования к оформлению приложения
- внешний вид приложения соответствует предложенному образцу или является его улучшенной версией
- вёрстка адаптивная. Минимальная ширина страницы, при которой проверяется корректность отображения приложения - 500рх, максимальная ширина страницы, при которой проверяется корректность отображения приложения - 1920рх
- интерактивность элементов, с которыми пользователи могут взаимодействовать, изменение внешнего вида самого элемента и состояния курсора при наведении, использование разных стилей для активного и неактивного состояния элемента, плавные анимации
- в футере приложения есть ссылка на гитхаб автора, год создания приложения, [логотип курса](https://rs.school/images/rs_school_js.svg) со [ссылкой на курс](https://rs.school/js/)

## Как сабмитить задание
Засабмитить задание необходимо как можно раньше, как только в rs app появится такая возможность. Для этого зайдите в rs app https://app.rs.school/, выберите пункт Cross-Check: Submit, в выпадающем списке выберите название таска, в поле Solution URL добавьте ссылку на задеплоенную версию вашего приложения, нажмите кнопку Submit.   
После сабмита задания его можно продолжать выполнять до самого дедлайна.

## Материалы
- [Официальная документация TypeScript](https://www.typescriptlang.org/)
- [Руководство по TypeScript](https://metanit.com/web/typescript/)
- [Практическое руководство по TypeScript для разработчиков](https://habr.com/ru/company/macloud/blog/557996/)
- [TypeScript - Быстрый Курс за 70 минут](https://youtu.be/nyIpDs2DJ_c)

## Cross-check
- инструкция по проведению cross-check: https://docs.rs.school/#/cross-check-flow
<!-- - ссылки на лучшие работы добавьте, пожалуйста, в эту форму 
- документ для вопросов:  -->
