# Трансформации

## 1. Подготовка

Нарисуем землю, два дерева и героя сказки;

## 2. Перемещения

Значение функции трансформации численное, а возможные единицы измерения — px, %, em или in. 

```
transform: translateX(-100px) // перемещение по оси Х, минус влево и плюс вправо
transform: translateY(-100px) // перемещение по оси У, минус вверх и плюс вниз
transform: translate(250px, -250px); // перемещение по двум осям
```

Делаем перемещение героя по земле.

Но он может и летать, добавим левитацию. Теперь он умеет летать. Будем перемещать его по воздуху (ось У).

Добавим ему фаерболл и цель, в которую он будет стрелять.

## 3. Увеличение, уменьшение

```
scale(масштаб-по-X [, масштаб-по-Y])
scale(0.5) уменьшит объект в 2 раза;
scale(2) увеличит объект в 2 раза;
scale(0) полностью «схлопнет» объект, и его не будет видно;
scale(1) оставит объект без изменений.
```

Добавим мышку и гиппопотама. Поиграем с размерами.

## 4. Вращение

Трансформация c функцией поворота `transform: rotate(угол наклона)`.

Положительное значение угла повернёт объект по часовой стрелке, а отрицательное — против. Единица измерения поворота — градусы deg, например: transform: rotate(180deg) повернёт объект на 180° по часовой стрелке, то есть перевернёт его.

Чтобы повёрнутый на 90° блок двигать по горизонтали, нужно применять translateY, а по вертикали — translateX.

Добавим дом, забор, волка.

## ЛАБИРИНТ

Реализуем перемещение героя по лабиринту.

```
.wizard-labirint {
  top: 344px;
  left: 10px;
  transform: translate(-20px, -150px) translate(310px, -110px) translate(200px, 260px);
}
```

Сделать - щелкаем по свитку, открывается карта.

## 5. Наклоны

Ещё одна возможность CSS-трансформаций — наклон объекта по осям X и Y под заданным углом. Наклоны создаются с помощью функций skewX и skewY.

Угол наклона задаётся в градусах — deg.
