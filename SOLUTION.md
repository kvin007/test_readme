
## 2. Instructions

You are working for a start-up that develops a photo app that is designed to take, edit, save and share pictures. 
Depending on the subscription plan, a user can have basic or plus features. Currently the design of the app follow 
the diagram below:

```mermaid
classDiagram
class PhoneCameraApp {
    +take() str
    +edit()* str
    +save() str
    +share()* str
}
class BasicCameraApp {
    +edit() str
    +share() str
}
class PlusCameraApp{
    +edit() str
    +share() str
}

PhoneCameraApp <|-- BasicCameraApp
PhoneCameraApp <|-- PlusCameraApp
```

