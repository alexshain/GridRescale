# GridInterpolate

## Описание
Данная программа предоставляет функционал для интерполяции одномерной сетки:
1. Интерполяционные методы:
    1.1. Интерполяция по ближайшему соседу (класс ClosestNeighborGridInterpolation)
    1.2. Линейная интерполяция (класс LinearGridInterpolation)

2. Класс Grid имеет методы upscale и downscale:
    2.1. Оба метода принимают на вход цело число k и указатель на полиморфный интерфейс IGridInterpolation
    2.2. Метод upscale возвращает сетку с шагом в k раз больше чем у исходной сетки и значениями сеточной функции, полученными соответствующей реализацией интерфейса IGridInterpolation
    2.3. Downscale – аналогично, но шаг в k раз меньше

## 📋 Требования

- **C++ 20** (совместимый компилятор: GCC 10+, Clang 10+, MSVC 19.28+)
- **CMake 3.10+**

## 🚀 Инструкция по сборке

### 1️⃣ Клонирование репозитория

```sh
git clone https://github.com/your-repo/project.git
cd project
```

### 2️⃣ Сборка

```sh
mkdir build && cd build
cmake ..
make
```

### 3️⃣ Запуск программы

```sh
./Rescale
```
