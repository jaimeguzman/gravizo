gravizo
=======

How to include graphviz graphs in github README.md

###New. The indirect way (required after github markdown engine change).###

You can use indirect way to refer a source file as graph description. 
![Alt text](https://g.gravizo.com/source/svg/custom_mark2?https%3A%2F%2Fraw.githubusercontent.com%2FTLmaK0%2Fgravizo%2Fmaster%2FREADME.md)
<!---
custom_mark2
@startuml
object Object01
object Object02
object Object03
object Object04
object Object05
object Object06
object Object07
object Object08

Object01 <|-- Object02
Object03 *-- Object04
Object05 o-- "4" Object06
Object07 .. Object08 : some labels2
@enduml
custom_mark2
-->

Use this sintax: ```![Alt text](https://g.gravizo.com/source/svg/<custom_mark>?<url_source_url_encoded>```). And use html comments ```<!--- -->``` to hide the source.
```
![Alt text](https://g.gravizo.com/source/svg/custom_mark?https%3A%2F%2Fraw.githubusercontent.com%2FTLmaK0%2Fgravizo%2Fmaster%2FREADME.md)
<!---
custom_mark
@startuml
object Object01
object Object02
object Object03
object Object04
object Object05
object Object06
object Object07
object Object08

Object01 <|-- Object02
Object03 *-- Object04
Object05 o-- "4" Object06
Object07 .. Object08 : some labels
@enduml
custom_mark
-->
```
