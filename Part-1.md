# **Redux**
### В чем особенности архитектуры Redux.
https://habr.com/ru/articles/464561/
___
### На какой базовой идее Redux основан. 
State машина

___
### local store и global store в проекте.
___

# **SwiftUI**

### Что такое View?
Протокол.
```Swift
public protocol View {
  associatedtype Body : View
  @ViewBuilder @MainActor var body: Self.Body { get }
}
```
___

### Как создать переиспользуемый компонент View, который может принимать различные параметры или данные?
Делаем структуру, подписываем на протокол Veiw.  Можно добавить `init()` в стуктуру.
___

### Что такое ViewBuilder?
https://habr.com/ru/articles/761722/
___

### В чем основное различие между HStack, VStack и ZStack в SwiftUI, и для чего каждый из них предназначен?
Это все контейнеры для группировки  View  
HStack - горизонтальная.
VStack - вертикальная.  
ZStack - "наслоение" одной View сверху другой. Как zPosition у layer в UIKit.  
___

### Какой модификатор позволяет контролировать пространство между элементами в HStack или VStack?
  `VStack(spacing: 33.0)`
___

### Что такое Spacer в SwiftUI и для каких целей он обычно используется?
  `Spacer()` - Пустая, адаптивная View, которая занимает все возможное пространство.  
___

### Можно ли изменять размер или другие свойства Spacer? Если да, то каким образом?
  `minlenght` - Spacing(), можно задать при создании.  
  `.frame()` - от View
___

### Как можно изменить шрифт, цвет и выравнивание текста в компоненте Text?
  `.font()`  
  `.foregroundColor()`  
  `.multilineTextAlignment()`
___

### Как загрузить изображение из ресурсов приложения с использованием компонента Image?
  `Image(_ name: String, bundle: Bundle? = nil)` - передать название файла строкой при созднии. Еще есть другие констукторы.  

  `Image(systemName: String)` - SF symbols.
___

### Как использовать кастомные View для представления кнопки, вместо стандартного представления?
  .onTapGesture {}   
___

### Как обработать ситуацию, когда изображение не может быть загружено или отображено?
___

### Что делает модификатор padding в SwiftUI и каковы его основные параметры?
`.padding(.bottom, 100)`  
___

### Как отступы влияют на размер и положение элемента View?
___

### Как задать отступ только с одной стороны элемента View?
___

### Что происходит, если применить модификатор padding к элементу несколько раз?
___

### Какие основные значения alignment можно использовать с HStack, VStack и ZStack?
  `.leading`  
  `.centr`  
  `.trailing`
___

### Как комбинирование padding и alignment может влиять на представление и положение View?
___

### Как добавить жест к элементу View в SwiftUI?
  `Gesture`  
___

### Как сочетать несколько жестов для одного элемента View?
  `simultaneousGesture()`
  
### Как реализовать действие, которое будет выполнено после долгого нажатия на элемент?
  `onlongpressgesture()`  
___

### Как разрешить конфликт, если два жеста могут быть распознаны одновременно?
___

### Как можно интегрировать SwiftUI View внутри UIKit UIViewController?
`UIHostingController()`  
https://developer.apple.com/documentation/swiftui/uihostingcontroller
___

### Как можно интегрировать UIKit компонент, например, UIView или UIViewController, внутри SwiftUI View?
Протокол UIViewRepresentable  
Пример:
```Swift
struct TextView: UIViewRepresentable {
  @Binding var text: NSMutableAttributedString
  
  func makeUIView(context: Context) -> UITextView {
    UITextView()
  }

  func updateUIView(_ uiView: UITextView, context: Context) {
      uiView.attributedText = text
  }
}
```
```Swift
struct ContentView: View {
  @State var text = NSMutableAttributedString(string: "")

  var body: some View {
      TextView(text: $text)
          .frame(minWidth: 0, maxWidth: .infinity, minHeight: 0, maxHeight: .infinity)
    }
}
```
https://www.hackingwithswift.com/quick-start/swiftui/how-to-wrap-a-custom-uiview-for-swiftui
___