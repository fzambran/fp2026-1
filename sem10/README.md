# Estructuras de Control — Secuenciales y Condicionales

Presentación en formato Quarto RevealJS para la semana 10 del curso **Fundamentos de Programación** (FP2026-1), Universidad Alberto Hurtado.

**Autor:** Felipe Zambrano B.  
**Fecha:** 11-05-2026

---

## Resultado de aprendizaje

Construir estructuras condicionales correctamente indentadas, tomando decisiones computacionales basadas en condiciones múltiples usando Python.

---

## Contenido de la presentación

### 1. ¿Qué son las Estructuras de Control?
Introducción a los tres tipos de estructuras de control en Python: secuenciales, condicionales y repetitivas. La unidad se enfoca en las dos primeras.

### 2. Estructura Secuencial
Descripción de la ejecución línea a línea: todas las instrucciones se ejecutan exactamente una vez, sin bifurcaciones. Ejemplo con `input()` y `print()`.

### 3. La instrucción `if`
Sintaxis y funcionamiento del `if` simple: evaluación de una condición booleana y ejecución condicional del bloque indentado. Incluye diagrama de flujo Mermaid.

**Ejemplo 1 — Verificación de nombre:** sistema que permite o deniega el acceso según el nombre ingresado.

### 4. La instrucción `if / else`
Extensión del `if` con rama alternativa `else`. Garantiza que siempre se ejecute exactamente uno de los dos bloques. Incluye diagrama de flujo Mermaid.

**Ejemplo 2 — Gatos o Perros:** el programa responde de forma distinta según la preferencia del usuario.

### 5. La indentación en Python
La indentación es parte de la sintaxis, no es opcional. Se cubren:
- Regla de los 4 espacios (PEP 8)
- Consistencia entre tabs y espacios
- `IndentationError` como consecuencia de errores

### 6. Errores comunes de indentación
Ejemplos comparativos de código incorrecto (sangría inconsistente, falta de `:`) versus código correcto.

### 7. La instrucción `if / elif / else`
Evaluación en cadena de múltiples condiciones. Python ejecuta solo el primer bloque cuya condición sea verdadera. El `else` captura todos los casos no cubiertos.

**Ejemplo 3 — Clasificación por edad:** categoriza al usuario en niño, adolescente, adulto o adulto mayor.

**Ejemplo 4 — Días de la semana:** mapea un número del 1 al 7 al nombre del día, con validación de entrada mediante `else`.

### 8. Condicionales anidados
Un `if` dentro de otro `if` permite decisiones en múltiples niveles. Se recomienda no superar 3 niveles de anidamiento.

**Ejemplo 5 — Validación académica:** aprobación según nota de presentación (≥ 4) y asistencia (≥ 70 %).

**Ejemplo 6 — Clasificación por generación:** identifica la generación (X, Millennials, Z, Alfa) a partir del año de nacimiento, usando rangos inclusivos (`1965 <= anio <= 1980`).

### 9. Expresiones condicionales (operador ternario)
Sintaxis de una línea para asignaciones simples:
```python
variable = valor_si_true if condición else valor_si_false
```
Útil para casos simples; se desaconseja para lógica compleja.

**Ejemplo 7 — Operador ternario en práctica:** par/impar, mayoría de edad y comparación de dos números.

### 10. Buenas prácticas
Tabla de recomendaciones: qué hacer (4 espacios, incluir `else`, limitar anidamiento) y qué evitar (mezclar tabs/espacios, olvidar `:`, operador ternario en lógica compleja).

### Resumen
Tabla de referencia rápida con todas las estructuras cubiertas y su uso principal.

---

## Estructura del repositorio

```
sem10/
├── estructuras_condicionales.qmd   # Fuente de la presentación (Quarto)
├── estructuras_condicionales.html  # Presentación RevealJS generada
├── uah.scss                        # Estilos personalizados UAH
├── pyproject.toml                  # Dependencias del entorno Python
└── uv.lock                         # Lock file de uv
```

## Cómo generar la presentación

```bash
quarto render estructuras_condicionales.qmd
```

Requiere [Quarto](https://quarto.org/) instalado y las dependencias de Python definidas en `pyproject.toml`.
