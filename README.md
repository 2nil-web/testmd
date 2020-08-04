#### Graphe hiérarchique ###
```mermaid
graph TD;
    WATT-->Jira;
    WATT-->Confluence;
    WATT-->Simba;
```


#### Diagramme de séquence
```mermaid
sequenceDiagram
Alice->>Bob: Hello Bob
Note right of Bob: Thinking ...
Bob->>Alice: Hello Alice
```


#### Organigramme
```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
```


#### Diagramme de Gantt
```mermaid
gantt
dateFormat  YYYY-MM-DD
title Adding GANTT diagram functionality to mermaid

Section A section
Completed task                      :done,    des1, 2020-01-06,2020-01-08
Active task                         :active,  des2, 2020-01-09, 3d
Future task                         :         des3, after des2, 5d
Future task2                        :         des4, after des3, 5d

section Critical tasks
Completed task in the critical line :crit, done, 2020-01-06,24h
Implement parser and jison          :crit, done, after des1, 2d
Create tests for parser             :crit, active, 3d
Future task in critical line        :crit, 5d
Create tests for renderer           :2d
Add to mermaid                      :1d

section Documentation
Describe gantt syntax               :active, a1, after des1, 3d
Add gantt diagram to demo page      :after a1  , 20h
Add another diagram to demo page    :doc1, after a1  , 48h

section Last section
Describe gantt syntax               :after doc1, 3d
Add gantt diagram to demo page      : 20h
Add another diagram to demo page    : 48h
```


#### Diagramme d'état
```mermaid
stateDiagram
    [*] --> Still
    Still --> [*]

    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

#### Diagramme de classe 
```mermaid
classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```

#### Camembert
```mermaid
pie
    title Pie Chart
    "Dogs" : 186
    "Cats" : 75
    "Rats" : 150
```

