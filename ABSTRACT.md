Abstract классы - описывают сущность.
Пример: Сколько углов у геометрической фигуры нельзя, можно сказать сколько углов у конкретной фигуры треугольник или у квадрата.

Если класс содержит Abstract-ые методы, то такой класс должен быть Абстрактным.

abstract class Geometry{
    width:string;
    color:string;
    
    abstract draw(): void
}

class Line extends Geometry{
    x1:number;
    draw(){}
}

Если у нас есть какой либо abstract метод, то мы в дочернем классе должны вызвать его.

Еще примеры: 

abstract class Car{
    model:string;

    abstract go(): void;
    abstract stop(): void;
    abstract start(): void;
}

class Af extends Car{
    go(){}
    stop(){}
    start(){}
}

let gfg: Af = new Af()