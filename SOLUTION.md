
## 2. Instructions

You are working for a start-up that develops a photo app that is designed to take, edit, save and share pictures. 
Depending on the subscription plan, a user can have basic or plus features. Currently the design of the app follow 
the diagram below:

```mermaid
classDiagram

class PhoneCameraApp {
    -_edit_method EditMethod
    -_share_method ShareMethod
    +take() str
    +save() str
}

class EditMethod
<<interface>> EditMethod{
    +edit() str
}

class ShareMethod
<<interface>> ShareMethod{
    +edit() str
}


class BasicEditMethod{
    +edit() str
}

class PlusEditMethod{
    +edit() str
}

class BasicShareMethod{
    +share() str
}

class PlusShareMethod{
    +share() str
}

PhoneCameraApp *-- EditMethod
PhoneCameraApp *-- ShareMethod
EditMethod <|-- BasicEditMethod
EditMethod <|-- PlusEditMethod
ShareMethod <|-- BasicShareMethod
ShareMethod <|-- PlusShareMethod


```

