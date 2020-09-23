# Database test

## 1. Stelle Entitäten mittels Chen-Notation und Min,Max Notation dar. Wähle ein sinnvolles Beispiel!

1:1 Notation

Ein Auto hat ein Nummernschild.
Das Nummernschild ist bei jedem Auto einzigartig

1:n Notation
Eine Mutter kann mehr Kinder gebähren.
Ein Kind und seine/ihre Geschwister hat immer nur eine (leibliche) Mutter

n:m Notation

Mehrere Studenten haben mehrere Professoren und umgekehrt.


## Kann eine Beziehung Attribute haben?
Ja sofern man die Beziehung auf die Primärschlüssel beider Entitäten herunterbricht und diese dann selbst als eigene Entität ansieht. 

Prof--teach--Student .... teach wird zu Prof_Student mit den jeweiligen IDs beider Parteien und dem gemeinsamen Nenner (zB der Kurs) als Attribute


## Kann eine Beziehung Attribute haben?

Operation
Katalog
Datensicherung
Integritätssicherung
Zugriffskontrolle

## Nenne den Unterschied zwischen Konzeptuellen und Logischem Schema!

Ersteres befasst sih mit dem Konzept, also der Definition aller Entitäten, Beziehungen und Attribute. Das logische Schema gibt an wie bestimmte Datensätze oder Tabellen miteinander verknüpft sind

## Welche 3 Bestandteile gibt es im Entity Relationship Model?

Entitäten, Attribute, Beziehungen(mit Kardinalitäten)


## Welche Datentypen gibt es in MySQL? (Nenne mindestens 5)

Char, Varhar, Integer, Smallint, Tinyint

## Welche Arten von Schlüsseln gibt es und welche Eigenschaften besitzen diese?

1. Primärschlüssel: Einzigartig und statisch
2. Sekundärshlüssel: Ist quasi die sidechick des Primärschlüssels 
3. Fremdschlüssel: Zeigt auf den Primärschlüssel einer anderen Entität
4. Nicht-Schlüssel: Attribute die auf garnichts verweisen

## Welche Arten von Beziehungen gibt es? Zeichne für jede ein Beispiel auf.

1. A-1---1-B (1zu1)
2. A-1---n-B (1zuN)
3. A-n---m-B (NzuM)

## Was bedeutet der Begriff Kardinalität und welche Kardinalitäten gibt es?

Kardinalität ist ein Begriff zur Darstellung dem Mengenverhältnis von einer Entität zur anderen. (1:1,1:N,M:N)

## Was bedeutet der Begriff Datenintegrität und worin unterscheidet sich Integrität und referentielle Integrität?

Die Datenintegrität gibt Aufschluss über die Qualität einer DB(vermeidung von Redundanz und so Zeug), während die ref. Integrität besteht quasi aus Regelungen die eine Datenintegrität gewährleisten

## Erkläre die 3 Normalformen.

1. NF1: Die inkludierten Datensätze einer Datenbank sollten elemtar sein und nicht gestackt vorliegen
2. NF2: Alle nicht Schlüsselelemente sind vom gesamten Primärschlüssel abhängig
3. NF3: Alle nicht Schlüssel Elemente sind voneinander unabhängig

## Erkläre den Unterschied zwischen starken und Schwachen Entitäten und erstelle ein Beispiel.

Schwache Entitäten verfügen über keine eigenen Primärschlüssel und hängen dementsprechend von den starken ab.

## Welche Grundregeln gibt es im Relationenmodell? (Nenne mindestens 4)

Ist das nicht dieselbe Frage wie zuvor mit Codd?

Wenn nicht evtl: Zugriffskontrolle, Rebootmöglichkeiten, Datensicherung, der obligatorische Schmerz beim Elernen von Datenbanken.

## Wie löst man eine M:N Beziehung auf? Erstelle ein Beispiel.

Prof--teach--Student .... teach wird zu Prof_Student mit den jeweiligen IDs beider Parteien und dem gemeinsamen Nenner (zB der Kurs) als Attribute

## Welche Anomalien kennst du und was beschreiben sie?#

Insert: Wenn neue Infos hinzugefügt werden
Update: Wenn aktualisiert wird
Delete: Wenn informationen gelöscht werden