@startuml
title template pattern
class AbstractClass 
{
    +void TemplateMethod()
    #virtual Primitive1()
    #virtual Primitive2()
}
AbstractClass ..|> TemplateMethod
interface TemplateMethod
{
    Primitive1()
    Primitive2()
}
class Contreteclass1 
{
    #virtual Primitive1()
    #virtual Primitive2()
}
class Contreteclass2 
{
    #virtual Primitive1()
    #virtual Primitive2()
}
Contreteclass1 .. |> AbstractClass
Contreteclass1 .. |> AbstractClass
@enduml