# TASK4

> Лиханова Алевтина

## 1.

Вариант 12: соответствие 

## 2.

```
соответсвие
|| |||   |
со тве   и - 6 уникальных букв

т - 3
с - 2
о - 2
в - 2
е - 2
и - 1
```

## 3.



<img width="612" alt="Снимок экрана 2024-10-24 в 20 08 29" src="https://github.com/user-attachments/assets/a9d5d5d2-047a-4715-b6c9-b3cbc4988c24">



```
с - 01
о - 100
т - 00
в - 101
е - 110
и - 111
```

## 4.

Количество уникальных букв: `6`

Минимальное требуемое количество бит: `3`

Словарь:
```
с - 000
о - 001
т - 010
в - 011
е - 100
и - 101
```

## 5.

### Равномерное кодирование (8-битный код) по таблице ASCII (кодировка CP1251)


Словарь

https://ru.wikipedia.org/wiki/Windows-1251

```
с - F1 - 11110001
о - EE - 11101110
т - F2 - 11110010
в - E2 - 11100010
е - E5 - 11100101
и - E8 - 11101000
```

Кодирование
```
с - 11110001
о - 11101110
о - 11101110
т - 11110010
в - 11100010
е - 11100101
т - 11110010
с - 11110001
т - 11110010
в - 11100010
и - 11101000
е - 11100101

```

Результат
```
111100011110111011101110111100101110001011100101111100101111000111110010111000101110100011100101
```
Длина - `96` бит

### Равномерное кодирование (3-битный код) по своему словарю

Словарь
```
с - 000
о - 001
т - 010
в - 011
е - 100
и - 101
```

Кодирование
```
c - 000
о - 001
о - 001
т - 010
в - 011
е - 100
т - 010
с - 000
т - 010
в - 011
и - 101
е - 100
```

Результат
```
000001001010011100010000010011101100
```
Длина - `36` бит

### Кодирование Хаффмана

Словарь
```
с - 01
о - 100
т - 00
в - 101
е - 110
и - 111
```

Кодирование
```
с - 01
о - 100
о - 100
т - 00
в - 101
е - 110
т - 00
с - 01
т - 00
в - 101
и - 111
е - 110
```

Результат

```
0110010000101110000100101111110
```

Длина - `31` бит

## Результаты кодирования:

| Кодировка | Длина сообщения |
|-----------|-----------------|
| ASCII     | `96`            |
| 3BIT      | `36`            |
| Хаффман   | `31`            |
