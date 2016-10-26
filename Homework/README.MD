# OOAD-WEEK10 HOMEWORK
## Sequence DIAGRAM

  Sequence 1
  Code
```
@startuml
Jack ->x John
Jack -> John
Jack->> John
Jack -\ John
Jack \\- John
Jack //-- John

Jack ->o John
Jack o\\-- John

Jack <-> John
Jack <->o John
@enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK10/blob/master/Homework/sequence1.png?raw=true">

----------------------------------------------------------------
 Sequence 2
  Code
```
@startuml
John -[#red]> Genny : hello
Genny -[#0000FF]->John : Hi
@enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK10/blob/master/Homework/Sequence2.png?raw=true">

----------------------------------------------------------------
 Sequence 3
  Code
```
@startuml

title Simple communication

Jenny -> Jack: Greeting Request
Jack --> Jenny: Greeting Response

@enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK10/blob/master/Homework/sequence3.png?raw=true">

----------------------------------------------------------------
 Sequence 4
  Code
```
@startuml
Jack->Boo : hello
note left: Greeting 1

Boo->Jack : Hi
note right: Respond Greeting 1

Boo->Boo : I am thinking
note left
	I am bemoaning
end note
@enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK10/blob/master/Homework/sequence4.png?raw=true">

----------------------------------------------------------------
 Sequence 5
  Code
```
@startuml
skinparam sequenceArrowThickness 2
skinparam roundcorner 20
skinparam maxmessagesize 60
skinparam sequenceParticipant underline

actor User
participant "First Class" as A
participant "Second Class" as B
participant "Last Class" as C

User -> A: Planing
activate A

A -> B: Doing
activate B

B -> C: Checking
activate C
C --> B: WorkDone
destroy C

B --> A: Created
deactivate B

A --> User: Done
deactivate A

@enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK10/blob/master/Homework/sequence5.png?raw=true">

----------------------------------------------------------------
