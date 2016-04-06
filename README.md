<img src='http://g.gravizo.com/g?
@startuml;

abstract class AbstractList;
abstract AbstractCollection;
interface List;
interface Collection;

List <|-- AbstractList;
Collection <|-- AbstractCollection;

Collection <|- List;
AbstractCollection <|- AbstractList;
AbstractList <|-- ArrayList;

class ArrayList {;
Object[] elementData;
size%28%29;
};

enum TimeUnit {;
DAYS;
HOURS;
MINUTES;
};

@enduml
'>