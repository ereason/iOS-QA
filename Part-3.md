# **Жизненные циклы View UIView UIViewController UIApplication**
### Какой метод жизненного цикла UIViewController вызывается при первом отображении представления на экране?
loadView -> viewDidLoad -> viewWillAppear 
___


### В чем разница между viewDidLoad и viewWillAppear в UIViewController?
https://habr.com/ru/articles/654517/
___

### Какие действия следует выполнять в методе viewWillLayoutSubviews?
Вызывается, чтобы уведомить ViewController о том, что его view собирается разместить свои subviews.
Этот метод вызывается каждый раз, когда frame изменяется, например, при повороте экрана или, когда он помечен как needing layout(требующий компоновки). Это первый шаг, на котором bounds(границы) view являются окончательными.
Если вы не используете autoresizingMask или constraints, а размер view изменяется, вы, вероятно, захотите обновить subviews здесь.
___

### Как UIViewController отслеживает изменение ориентации устройства?
___

### В чем особенность использования loadView для инициализации представления UIViewController?
___

### Чем отличается поведение жизненного цикла представления при использовании контейнеров (например, UINavigationController или UITabBarController)?
___

### Какие события жизненного цикла приложения (UIApplication) вы знаете и как они взаимодействуют с жизненным циклом UIViewController?
___

### Какие события жизненного цикла приложения обрабатываются делегатом UIApplication и какие методы соответствуют этим событиям?
___

### Как можно отслеживать переход приложения между активным, фоновым и неактивным состояниями, и какие методы делегата UIApplication вызываются при этих переходах?
___

### Какие методы делегата UIApplication используются для обработки запуска приложения с определёнными параметрами, например, через URL-схемы или локальные уведомления?
___

### Как приложение может обрабатывать события, такие как низкий уровень заряда батареи или изменение времени, и в каких методах делегата UIApplication это следует делать?
___

### В каком методе жизненного цикла UIApplication следует сохранять критические данные и освобождать ресурсы перед тем, как приложение будет полностью закрыто или переведено в фоновый режим?
___

### Как SwiftUI определяет, что View нужно перерисовать, и как связаны с этим процессом свойства-обертки, такие как @State, @Binding, @ObservedObject и @EnvironmentObject?
___

### Каковы ключевые различия между @State и @ObservedObject в контексте жизненного цикла View и как они влияют на обновление представления?
___

### Как работает модификатор .onAppear и .onDisappear в жизненном цикле View и в каких случаях их следует использовать?
___

### Каковы лучшие практики управления ресурсами, например, отмена сетевых запросов или таймеров, в контексте жизненного цикла View?
___

### Как View может реагировать на изменения в глобальном окружении, например, на смену темы или изменение размера шрифта в настройках доступности, и какие модификаторы View поддерживают такие изменения?
___


# **Нажатие пользователя на уровне системы**

### Что такое responder chain в контексте iOS приложений?
___

### Как responder chain используется для обработки событий касаний?
___

### Каков порядок прохождения события нажатия через responder chain?
___

### Как объект может стать первым респондентом (first responder) в responder chain?
___

### Каким образом UIView может отказаться от статуса first responder?
___

### Какие методы UIResponder используются для обработки событий касания, таких как touchesBegan, touchesMoved, touchesEnded и touchesCancelled?
___

### Как UIViewController влияет на обработку событий в responder chain?
___

### Как события жестов интегрируются в responder chain?
___

### Как определить, должен ли объект UIView получить событие касания?
___

### В чем разница между responder chain и event handling в UIKit?
___

### Как управлять responder chain, чтобы кастомизировать обработку событий в сложных иерархиях представлений?
___

### Могут ли не-представления (non-views), такие как UIViewController или UIApplication, стать частью responder chain?
___

### Как можно программно заставить UIView стать первым респондентом?
___

### Какие сценарии могут привести к тому, что UIView потеряет статус первого респондента?
___

### Как изменение first responder влияет на визуальное состояние интерфейса, например, на появление и скрытие клавиатуры?
___


# **Сеть**

### Что такое URLSession и для каких задач он используется в iOS?
___

### Какие основные компоненты URLSession и как они взаимодействуют друг с другом?
___

### Какие типы задач (tasks) поддерживает URLSession и в чем их отличия?
___

### Как создать и настроить URLSessionConfiguration для настройки поведения сессии?
___

### Как можно отправить простой GET запрос с использованием URLSession?
___

### Как обрабатывать ответы сервера и данные, полученные в результате URLSessionDataTask?
___

### Как можно загрузить файл на сервер, используя URLSessionUploadTask?
func uploadTask(with: URLRequest, from: Data) -> URLSessionUploadTask
___

### Как в URLSession использовать URLSessionDownloadTask для загрузки файлов и обработки прогресса загрузки?
Download tasks directly write the server’s response data to a temporary file, providing your app with progress updates as data arrives from the server. When you use download tasks in background sessions, these downloads continue even when your app is in the suspended state or otherwise not running.
___

### Как можно обрабатывать многозадачность и продолжение передачи данных в фоновом режиме с помощью URLSession?
___

### Как реализовать обработку сетевых ошибок и статусных кодов HTTP при использовании URLSession?
___

### Как использовать URLSession для работы с WebSocket соединениями?
___

### Как управлять кэшированием ответов в URLSession?
___

### Какие есть способы аутентификации и авторизации при использовании URLSession?
___

### Как настроить таймауты для сетевых запросов в URLSession?
___

### Как реализовать отмену сетевых запросов и управление их приоритетами в URLSession?
___


# **Appearance**

### Что такое Appearance API в iOS и для чего он используется?
___

### Как изменить глобальный внешний вид всех экземпляров определенного класса UIView?
___

### Могут ли индивидуальные экземпляры UIView иметь свой уникальный внешний вид, отличный от глобального Appearance?
___

### Как можно настроить Appearance для навигационной панели в UINavigationController?
UINavigationBarAppearance
___

### Как Appearance влияет на элементы управления, такие как UIButton или UILabel?
 UIButton.appearance().backgroundColor = .black
___

### Какие свойства можно настроить с помощью UIAppearance?
___

### Как программно переключаться между светлой и темной темами в приложении?
___

### Как Appearance связан с поддержкой темной темы в iOS?
___

### Как настроить внешний вид UITabBar с помощью Appearance API?
___

### Как изменить стиль курсора для конкретного UIView с использованием Appearance?
___

### Можно ли настроить Appearance элементов, которые находятся внутри UIPopoverController?
___

### Как установить специфический внешний вид для UIAlertController?
___

### Как использовать UIAppearance для изменения внешнего вида UISearchBar?
You can customize the appearance of search bars one at a time, or you can use the appearance proxy ([UISearchBar appearance]) to customize the appearance of all search bars in an app.
In general, you should specify a value for the normal state to be used by other states which don’t have a custom value set. Similarly, when a property is dependent on the bar metrics (on iPhone, in landscape orientation bars have a different height from standard), you should specify a value for UIBarMetricsDefault.
___

### Как изменить внешний вид стандартных кнопок системы, таких как кнопки в UIAlertController?
___

### Влияет ли изменение Appearance на уже отображаемые на экране элементы интерфейса или только на те, что будут созданы и отображены в будущем?
___

### Как связаны UIKit appearance и SwiftUI элементы
___