# Recursos Adicionales 📚

Aquí encontrarás materiales complementarios para profundizar en lo que aprendiste.

## 1. Guía Rápida de Referencia

### Python Básico
```python
# Variables
nombre = "Ana"
edad = 25

# Tipos de datos
texto = "string"
numero = 42
decimal = 3.14
booleano = True/False

# Operaciones
suma = 10 + 5              # 15
resta = 10 - 5             # 5
multiplicacion = 10 * 5    # 50
division = 10 / 5          # 2.0
potencia = 2 ** 3          # 8
modulo = 10 % 3            # 1 (resto)
```

### Listas
```python
lista = [1, 2, 3, 4, 5]
primer = lista[0]          # 1
ultimo = lista[-1]         # 5
sub_lista = lista[1:3]     # [2, 3]

lista.append(6)            # Agregar
lista.remove(3)            # Eliminar
longitud = len(lista)      # 5
```

### Bucles
```python
# Bucle for con range
for i in range(5):
    print(i)               # 0, 1, 2, 3, 4

# Bucle for con lista
for elemento in [1, 2, 3]:
    print(elemento)

# Bucle while
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

### Condicionales
```python
if x > 10:
    print("Mayor que 10")
elif x > 5:
    print("Mayor que 5")
else:
    print("Menor o igual a 5")
```

### Funciones
```python
def sumar(a, b):
    return a + b

resultado = sumar(5, 3)    # 8

def saludar(nombre="Amigo"):
    print(f"¡Hola, {nombre}!")

saludar("María")           # ¡Hola, María!
saludar()                  # ¡Hola, Amigo!
```

---

## 2. Pandas - Operaciones Comunes

### Cargar Datos
```python
import pandas as pd

df = pd.read_csv('archivo.csv')
df = pd.read_excel('archivo.xlsx')
df = pd.read_json('archivo.json')
```

### Explorar
```python
df.head()              # Primeras filas
df.tail()              # Últimas filas
df.shape               # (filas, columnas)
df.info()              # Información
df.describe()          # Estadísticas
df.columns             # Nombres de columnas
df.dtypes              # Tipos de datos
```

### Acceder a Datos
```python
df['columna']          # Acceder a columna
df.loc[0]              # Acceder por índice
df.iloc[0, 1]          # Acceder por posición
df[df['col'] > 5]      # Filtrar
```

### Estadísticas
```python
df['col'].mean()       # Promedio
df['col'].median()     # Mediana
df['col'].std()        # Desviación estándar
df['col'].min()        # Mínimo
df['col'].max()        # Máximo
df['col'].sum()        # Suma
df['col'].count()      # Cantidad
```

### Transformar
```python
df['nueva'] = df['col'] * 2              # Nueva columna
df = df.drop('col', axis=1)              # Eliminar columna
df = df.rename(columns={'old': 'new'})   # Renombrar
df = df.sort_values('col')               # Ordenar
```

### Agrupar
```python
df.groupby('categoria')['valor'].mean()
df.groupby('categoria').size()
df.groupby('cat').agg({'valor': ['sum', 'mean', 'max']})
```

---

## 3. Matplotlib - Gráficos Básicos

```python
import matplotlib.pyplot as plt

# Gráfico de líneas
plt.plot([1, 2, 3, 4], [1, 4, 2, 3])
plt.title("Mi Gráfico")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")
plt.show()

# Gráfico de barras
plt.bar(['A', 'B', 'C'], [10, 20, 15])
plt.show()

# Histograma
plt.hist([1, 1, 2, 2, 2, 3, 3, 3, 3])
plt.show()

# Dispersión
plt.scatter([1, 2, 3], [1, 4, 2])
plt.show()
```

---

## 4. Errores Comunes y Soluciones

| Error | Causa | Solución |
|-------|-------|----------|
| `NameError` | Variable no definida | Verifica la sintaxis del nombre |
| `IndexError` | Índice fuera de rango | Usa índices válidos (0 a len-1) |
| `KeyError` | Columna no existe | Verifica el nombre exacto de la columna |
| `TypeError` | Tipo de dato incorrecto | Convierte al tipo adecuado |
| `FileNotFoundError` | Archivo no existe | Verifica la ruta |

---

## 5. Atajos Útiles en Notebooks

| Acción | Atajo |
|--------|-------|
| Ejecutar celda | Shift + Enter |
| Ejecutar todas | Ctrl + Shift + Enter |
| Nueva celda abajo | Alt + Enter |
| Nueva celda arriba | Ctrl + Shift + A |
| Eliminar celda | D + D |
| Cambiar a Markdown | M |
| Cambiar a Código | Y |
| Comentar | Ctrl + / |

---

## 6. Recursos en Línea

### Documentación Oficial
- **Python**: https://docs.python.org/3/
- **Pandas**: https://pandas.pydata.org/docs/
- **Matplotlib**: https://matplotlib.org/stable/contents.html
- **NumPy**: https://numpy.org/doc/

### Tutoriales
- **Real Python**: https://realpython.com/
- **DataCamp**: https://www.datacamp.com/
- **Kaggle Learn**: https://www.kaggle.com/learn

### Comunidades
- Stack Overflow
- GitHub
- Reddit (r/learnprogramming)

---

## 7. Proyectos de Práctica

Aquí hay ideas de proyectos que puedes hacer:

### Nivel 1: Básico
- [ ] Crear un programa que calcule el IMC
- [ ] Analizar datos de tu disciplina
- [ ] Crear un juego de adivinanzas en Python

### Nivel 2: Intermedio
- [ ] Descargar datos públicos y analizarlos
- [ ] Crear gráficos interactivos
- [ ] Limpiar datos con valores faltantes

### Nivel 3: Avanzado
- [ ] Aplicar machine learning básico
- [ ] Crear un dashboard
- [ ] Automatizar tareas rutinarias

---

## 8. Consejos Prácticos

### Para Escribir Mejor Código
✓ Usa nombres descriptivos para variables  
✓ Comenta el código complejo  
✓ Mantén el código limpio y organizado  
✓ Prueba pequeñas partes antes de juntar todo  

### Para Aprender Más Rápido
✓ Practica regularmente  
✓ Lee código de otros  
✓ Experimenta modificando ejemplos  
✓ Enseña a otros lo que aprendes  

### Para Debuggear
✓ Usa `print()` para verificar valores  
✓ Lee el mensaje de error cuidadosamente  
✓ Busca el error online  
✓ Pregunta en comunidades  

---

## 9. Glosario de Términos

| Término | Significado |
|---------|------------|
| Variable | Contenedor de datos |
| Función | Conjunto reutilizable de instrucciones |
| Bucle | Repetición de acciones |
| Condicional | Decisión (if/else) |
| Lista | Colección ordenada |
| Diccionario | Colección clave-valor |
| DataFrame | Tabla de datos (Pandas) |
| Índice | Posición en una lista (comienza en 0) |
| Método | Función de un objeto |
| Biblioteca | Colección de código reutilizable |

---

## 10. Plantilla para Comenzar un Nuevo Análisis

```python
# Importar bibliotecas
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Cargar datos
df = pd.read_csv('mis_datos.csv')

# Explorar
print(f"Dimensiones: {df.shape}")
print(df.head())
print(df.info())

# Limpiar (si es necesario)
df = df.dropna()

# Analizar
print(df.describe())

# Visualizar
df.plot(kind='bar')
plt.show()

# Guardar resultados
# df.to_csv('resultados.csv', index=False)
```

---

## 11. Preguntas de Autoevaluación

Prueba si entendiste:

- ¿Puedo explicar qué es una variable?
- ¿Entiendo la diferencia entre listas y diccionarios?
- ¿Sé cómo cargar datos con Pandas?
- ¿Puedo filtrar datos?
- ¿Sé crear un gráfico básico?
- ¿Entiendo qué es un bucle?
- ¿Sé cómo usar condicionales?

Si respondiste **No** a alguna, vuelve a revisar el material correspondiente.

---

## 12. Contacto y Preguntas

Si tienes dudas:

1. **Revisa los ejemplos** en `01_ejemplos.ipynb`
2. **Consulta esta guía** de referencia
3. **Lee las soluciones** en `02_ejercicios.ipynb`
4. **Experimenta** modificando el código
5. **Busca** la solución online (hay muchos recursos)

---

**¡Recuerda!** La mejor forma de aprender es haciendo. No temas cometer errores; ¡son parte del aprendizaje!

*Última actualización: Septiembre 2026*
