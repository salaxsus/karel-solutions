# 1.2.2 fillTheHoles

## Lösung

```java
void fillTheHoles() {
    repeat (4) {
        moveForward();
        fillHole();
        moveForward();
    }
}

void fillHole() {
    turnRight();
    moveForward();
    dropBeeper();
    turnAround();
    moveForward();
    turnRight();
}
```
