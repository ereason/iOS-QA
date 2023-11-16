# **Архитектура приложений**

### Какие особенности у MVVM MVP VIPER архитектуре применительно к iOS
View–Interactor–Presenter–Entity–Router.
https://habr.com/ru/companies/badoo/articles/281162/
___


### Что такое Unidirectional Data Flow и для чего нужен
https://habr.com/ru/companies/inDrive/articles/571394/
___

### Что такое доменный слой и для чего он нужен
В доменном слое находятся код и данные из предметной области приложения.
Бизнес логика
___

### SOLID расшифровка каждого пункта 
single responsibility, open–closed, Liskov substitution, interface segregation и dependency inversion
___

### DRY KISS YAGNI
dont repeat yourself
keep it simple
yr not gonna need it

https://habr.com/ru/companies/itelma/articles/546372/
___

### Как внедрение зависимостей (dependency injection) способствует созданию модульного и тестируемого кода?
быстрая подмена
___

### Шаблоны проектирования на какие группы делятся, назовите по несколько штук в каждой группе. В стандартной архитектуре Apple какие шаблоны часто встречаются?
___

# **@State Bindning и другие модификаторы в SwiftUI**


### Как работает модификатор @State в SwiftUI и для чего он обычно используется?
https://www.hackingwithswift.com/quick-start/swiftui/what-is-the-state-property-wrapper
___

### Как можно связать данные, хранящиеся в @State переменной, с элементом пользовательского интерфейса?
___

### В чем разница между @State и @Binding?
https://stackoverflow.com/questions/59247183/swiftui-state-vs-binding
___

### Как можно создать двустороннюю привязку (Binding) к @State переменной?
___

### Какие ограничения существуют при использовании @State переменных?
___

### Почему @Binding не требует инициализатора, а @State требует?
___

### В чем разница между @State и @ObservedObject?
___

### Чем @EnvironmentObject отличается от @Binding и когда его следует использовать?
___

### Как передать @Binding переменную между двумя view?
___

### Что происходит с состоянием view, когда используется модификатор @State, и это view исчезает из иерархии представлений?
___

### Можно ли использовать @State для хранения сложных типов данных, таких как пользовательские классы или структуры?
___

### Как изменение @State переменной влияет на жизненный цикл view?
___

### Почему изменения @Binding переменной могут привести к перерисовке view?
___

### Как модификатор @State используется для управления показом модального окна?
___

### Какой модификатор следует использовать для управления фокусом на текстовом поле в SwiftUI?
___


# **ScrollView LazyGrid**

### В чем основное назначение компонента ScrollView в SwiftUI?
https://developer.apple.com/documentation/swiftui/scrollview
___

### Какие основные параметры конструктора ScrollView?
init(Axis.Set, showsIndicators: Bool, content: () -> Content)
___

### Как можно создать горизонтальный ScrollView?
в констуктор
___

### Что такое LazyVGrid и LazyHGrid и в чем отличие их от обычных VGrid и HGrid?
https://developer.apple.com/documentation/swiftui/lazyvgrid
___

### Как управлять пространством между строками и столбцами в LazyVGrid или LazyHGrid?
let rows = [GridItem(.fixed(30)), GridItem(.fixed(30))]
GridItem
___

### Как LazyGrid управляет памятью и производительностью при прокрутке большого количества элементов?
___

### Какова цель использования LazyGrid вместо обычного Grid?
___

### Можно ли создать динамически изменяющееся количество столбцов в LazyGrid на основе размера экрана?
___

### Каким образом можно реализовать пагинацию или бесконечную прокрутку в ScrollView?
___

### Можно ли использовать LazyGrid для создания сложных макетов с неоднородными размерами ячеек?
___

### Каким образом можно добавить обновление данных при "pull to refresh" в ScrollView?
GeometryReader
___

### В чем отличие использования ScrollView и List для отображения вертикального списка элементов?
pull to refresh
___

### Как можно интегрировать LazyGrid в ScrollView, чтобы иметь возможность вертикально прокручивать как саму сетку, так и другие элементы?
___

### Можно ли добавить секционные заголовки в LazyVGrid или LazyHGrid?
___

### Как обрабатывать событие нажатия на элемент внутри LazyGrid?
