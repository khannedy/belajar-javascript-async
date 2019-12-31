```puml
@startuml

participant "Main Thread" as App
participant "Web Worker Thread" as WebWorker

activate App
App --> WebWorker : Post Message
activate WebWorker
App -> App : Show Header
WebWorker --> WebWorker : Do Work
App -> App : Show Footer
WebWorker --> App : Post Message
deactivate WebWorker
deactivate App

@enduml
```
