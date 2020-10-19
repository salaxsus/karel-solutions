# 3.1.1 partyAgain

## Lösung

```java
void partyAgain() {
    while (frontIsClear()) {
        column();
        moveForward();
    }
    column();
}

void column() {
    turnLeft();
    pickBeeper();
    walkAndPick();
    turnLeft();
}

void walkAndPick() {
    if (frontIsClear()) {
        walk();
    } else {
        dropBeeper();
        turnAround();   
    }
}

void walk() {
    moveForward();
    walkAndPick();
    moveForward();
}
```
