# sass-bitwise

**A library of 32-Bit Bitwise Operations implemented fully in SASS.**

Works similar to standard JavaScript Bitwise Operations. The library assumes inputs are positive integars, but all bitwise operations are performed on 32 bits binary numbers. Before a bitwise operation is performed, the library converts numbers to 32 bits signed integers. After the bitwise operation is performed, the result is converted back to SASS numbers.

## Installation

This library can be installed using NPM.

```
npm install sass-bitwise
```

## Usage

> If you are having problems with your imports you may need to use the full path:
>
> ```scss
> @use "../node_modules/sass-bitwise" as bitwise;
> ```

### Bitwise NOT ( ~ )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitNot(2863311530);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitNot(2863311530)
```

Ouput

```
1431655765
```

### Bitwise AND ( & )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitAnd(763, 93);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitAnd(763, 93)
```

Ouput

```
89
```

### Bitwise OR ( | )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitOr(763, 93);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitOr(763, 93)
```

Ouput

```
767
```

### Bitwise XOR ( ^ )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitXor(763, 93);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitXor(763, 93)
```

Ouput

```
678
```

### Bitwise Left Shift ( << )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitLShift(763, 3);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitLShift(763, 3)
```

Ouput

```
6104
```

### Bitwise Arithmetic Right Shift ( >> )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitSignShift(763, 3);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitSignShift(763, 3)
```

Ouput

```
95
```

### Bitwise Logical Right Shift ( >>> )

SCSS

```scss
@use "bitwise" as bitwise;

@debug bitwise.bitRShift(763, 3);
```

SASS

```sass
@use 'bitwise' as bitwise

@debug bitwise.bitRShift(763, 3)
```

Ouput

```
95
```
