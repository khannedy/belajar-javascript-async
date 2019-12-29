```puml
@startuml

participant "Main Thread" as App

activate App
App -> App : Get Product by Id
App -> App : Show Product
App -> App : Show Header
App -> App : Show Footer 
deactivate App

@enduml
```
