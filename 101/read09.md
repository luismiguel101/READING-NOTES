# Fundamentos de JavaScript

## Tipos de datos en JavaScript

JavaScript tiene varios tipos de datos primitivos y estructurados:

- **Primitivos:**
  - `String`: Cadenas de texto (Ejemplo: `'Hola'`, `"Mundo"`)
  - `Number`: Números enteros y decimales (Ejemplo: `42`, `3.14`)
  - `Boolean`: Verdadero o falso (`true` o `false`)
  - `Undefined`: Valor por defecto de una variable no inicializada
  - `Null`: Representa la ausencia de valor
  - `Symbol`: Identificadores únicos (usado en objetos)
  - `BigInt`: Números enteros grandes (Ejemplo: `9007199254740991n`)

- **Estructurados:**
  - `Object`: Conjunto de propiedades clave-valor
  - `Array`: Lista ordenada de valores
  - `Function`: Bloques reutilizables de código

## Estructuras condicionales en JavaScript

Las estructuras condicionales permiten ejecutar diferentes bloques de código según ciertas condiciones:

```js
let edad = 18;
if (edad >= 18) {
    console.log("Eres mayor de edad.");
} else {
    console.log("Eres menor de edad.");
}
```

### Propósito:
- Evaluar condiciones lógicas y tomar decisiones.
- Controlar el flujo del programa.

## Tipos de operadores en JavaScript

### Operadores aritméticos
Estos operadores permiten realizar cálculos matemáticos:

| Operador | Descripción | Ejemplo |
|----------|------------|---------|
| `+` | Suma | `5 + 3 // 8` |
| `-` | Resta | `10 - 2 // 8` |
| `*` | Multiplicación | `4 * 2 // 8` |
| `/` | División | `16 / 4 // 4` |
| `%` | Módulo (resto) | `10 % 3 // 1` |
| `**` | Potencia | `2 ** 3 // 8` |

Otros tipos de operadores incluyen:
- **Operadores de comparación** (`==`, `!=`, `===`, `!==`, `>`, `<`, `>=`, `<=`)
- **Operadores lógicos** (`&&`, `||`, `!`)
- **Operadores de asignación** (`=`, `+=`, `-=`, `*=`, etc.)

## Declaración de variables en JavaScript

JavaScript permite declarar variables con `var`, `let` y `const`:

```js
var nombre = "Juan"; // Variable global o función (evitar en ES6)
let edad = 25; // Variable de bloque, puede cambiar
const PI = 3.1416; // Constante, no puede cambiar
```

### Diferencias clave:

| Tipo | Alcance | Mutabilidad |
|------|---------|-------------|
| `var` | Global o de función | Se puede reasignar |
| `let` | De bloque | Se puede reasignar |
| `const` | De bloque | No se puede reasignar |

Usar `let` y `const` es recomendado en ES6 para evitar problemas de alcance y mejorar la legibilidad del código.
