___
### 5 часть
# UITableView
___
### Как UITableView решает проблему переиспользования ячеек при прокрутке для оптимизации производительности?
___
### Какие шаги нужно выполнить для настройки простого UITableView с пользовательскими ячейками в iOS?
___
### В чем разница между dequeueReusableCell(withIdentifier:) и dequeueReusableCell(withIdentifier:for:)?
___
### Как можно добавить действия к ячейке (например, свайп влево для удаления) в UITableView?
___
### Как вы можете программно переместить ячейку в UITableView?
___
### Как UITableView связывается с источником данных, и какие методы протокола UITableViewDataSource являются обязательными?
___
### Каким образом можно реализовать разные высоты ячеек в UITableView?
___
### Как вы можете использовать UITableView для отображения данных в нескольких секциях и как управлять заголовками и подвалами секций?
___
### Как реализовать "pull to refresh" функциональность в UITableView?
___
### Какие лучшие практики существуют для улучшения производительности прокрутки в UITableView, особенно при работе с большими объемами данных или сложными ячейками?
# UICollectionView
___
### Как реализовать многоколоночный макет в UICollectionView?
___
### В чем разница между UICollectionView и UITableView, и когда предпочтительнее использовать каждый из них?
___
### Какие шаги необходимо выполнить для создания пользовательских ячеек в UICollectionView?
___
### Как можно добавить заголовки и подвалы секций в UICollectionView?
___
### Как реализовать различные типы анимаций при добавлении, удалении или перемещении ячеек в UICollectionView?
___
### Как можно использовать UICollectionView для создания горизонтальной прокрутки?
___
### Как UICollectionView взаимодействует с UICollectionViewDataSource и UICollectionViewDelegate?
___
### Как изменить расстояние между ячейками и строками в UICollectionView?
___
### Какие методы нужно реализовать в UICollectionViewDataSource для поддержки выбора и выделения ячеек?
___
### Как реализовать drag-and-drop для переупорядочивания ячеек внутри UICollectionView?
___
### Как создать собственный подкласс UICollectionViewLayout для настройки уникального макета элементов?
___
### В чем разница между UICollectionViewFlowLayout и кастомным UICollectionViewLayout?
___
### Как UICollectionViewLayout влияет на поведение анимаций при добавлении или удалении ячеек?
___
### Как можно оптимизировать производительность UICollectionView, настроив свойство estimatedItemSize в UICollectionViewFlowLayout?
___
### Какие параметры нужно учитывать при расчете размеров и положения элементов в кастомном UICollectionViewLayout?
# Combine
___
### Каковы основные компоненты в архитектуре Combine?
___
### Как можно использовать Combine для управления асинхронным потоком данных?
___
### Какие операторы Combine можно использовать для преобразования потока данных?
___
### Как Combine обрабатывает ошибки в потоке данных?
___
### В чем разница между Future и Subject в Combine?
___
### Какие типы Subject предоставляет Combine и в чем их различие?
___
### Как можно использовать Combine для связывания UI компонентов с данными?
___
### Как реализовать back pressure в потоке данных с помощью Combine?
___
### Как использовать Combine для создания цепочек асинхронных операций?
___
### Какие есть способы отмены подписки на поток данных в Combine?
___
### Как использовать операторы debounce и throttle в Combine и в чем их 
___
### Как работает метод combineLatest в Combine и для решения каких задач он подходит?
___
### В чем разница между merge, combineLatest и zip?
___
### Как использовать switchToLatest для работы с динамически изменяющимися Publisher?
___
### Каким образом flatMap позволяет обрабатывать значения из нескольких Publisher?
___
### Какие есть способы ограничения количества значений, получаемых от Publisher?
___
### Как scan используется для агрегирования исходящих значений?
___
### Что такое Subject и какие основные типы Subject существуют в Combine?
___
### Как применять map и tryMap для преобразования значений в потоке?
___
### Как filter и tryFilter используются для управления потоком данных в Combine?
___
### Какие методы в Combine позволяют работать с потоками данных, которые могут завершаться ошибкой?
___
### Как handleEvents позволяет выполнить действия на различных этапах жизненного цикла Publisher?
___
### Как работает delay для отложенной отправки значений?
___
### Как collect позволяет группировать исходящие значения от Publisher?
___
### В чем различие между receiveOn и subscribeOn?
___
### Как breakpoint и breakpointOnError используются для отладки потока данных?
___
### Каким образом можно использовать removeDuplicates для предотвращения отправки повторяющихся значений?
___
### Как ignoreOutput используется для игнорирования всех значений от Publisher?
___
### Какие стратегии существуют в Combine для повторения неудачных операций?
___
### Работа с локальными и серверными пуш-уведомлениями
___
### Как можно настроить локальные уведомления в iOS?
___
### Какие основные отличия между локальными и серверными пуш-уведомлениями?
___
### Какие шаги необходимы для регистрации устройства на получение пуш-уведомлений?
___
### Какие изменения в настройках уведомлений пользователь может выполнить в iOS?
___
### Как можно обрабатывать пуш-уведомления, когда приложение находится в фоновом режиме?
___
### Как реализовать интерактивные уведомления с кнопками для выполнения действий?
___
### Как можно отправлять медиа-контент (изображения, видео) в пуш-уведомлениях?
___
### Как обрабатывать нажатия на уведомления для выполнения конкретных действий в приложении?
___
### Какие ограничения существуют на размер и содержимое пуш-уведомлений?
___
### Как обновлять или удалять отправленные пуш-уведомления?
___
### Как можно группировать уведомления от одного приложения?
___
### Как реализовать тихие уведомления (silent push notifications) и для чего они используются?
___
### Какие стратегии лучше использовать для сегментации и персонализации пуш-уведомлений?
___
### Какие данные стоит включать в пейлоад пуш-уведомлений для максимальной информативности?
___
### Каким образом iOS обрабатывает пуш-уведомления, когда приложение не запущено?
___
### Как ограничить количество пуш-уведомлений, чтобы избежать их избыточности для пользователя?
