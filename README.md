# Módulo 5: Herramientas de Investigación 🔍

¡Bienvenido al Módulo 5! Este módulo está diseñado para enseñarte los conceptos fundamentales de las herramientas de investigación basadas en Python, de manera simple e inclusiva para personas de todas las disciplinas.

---

## 📚 Contenidos del Módulo

Este módulo se divide en tres secciones principales:

### 1. **Cuadernos Interactivos (Notebooks)**
- **00_inicio.ipynb** - Comienza aquí: conceptos básicos de Python
- **01_ejemplos.ipynb** - Ejemplos prácticos paso a paso
- **02_ejercicios.ipynb** - Ejercicios para practicar

### 2. **Datos (Data)**
- Archivo `investigacion_datos.csv` con datos de ejemplo que usaremos en los ejercicios

### 3. **Recursos (Recursos)**
- Guías, referencias y materiales de apoyo

---

## 🎯 Objetivos de Aprendizaje

Al completar este módulo, podrás:

✓ Entender los conceptos básicos de Python para análisis de datos  
✓ Cargar y explorar datos usando bibliotecas como Pandas  
✓ Realizar operaciones simples de análisis de datos  
✓ Visualizar y entender patrones en los datos  
✓ Escribir código limpio y bien documentado  

---

## 🚀 Cómo Empezar

### Requisitos
- Python 3.7 o superior
- Bibliotecas: pandas, numpy, matplotlib (se instalan automáticamente)

### Pasos para Comenzar

1. **Abre el primer cuaderno**: `00_inicio.ipynb`
   - Familiarízate con la interfaz
   - Ejecuta el código paso a paso
   
2. **Estudia los ejemplos**: `01_ejemplos.ipynb`
   - Lee las explicaciones cuidadosamente
   - Modifica el código para experimentar
   
3. **Practica con ejercicios**: `02_ejercicios.ipynb`
   - Resuelve los problemas propuestos
   - No dudes en consultar los ejemplos

---

## 💡 Conceptos Clave

### Variables y Tipos de Datos
```python
nombre = "Juan"              # Texto (string)
edad = 25                    # Número entero (int)
altura = 1.75                # Número decimal (float)
es_estudiante = True         # Booleano (True/False)
```

### Operaciones Básicas
```python
suma = 10 + 5               # 15
resta = 10 - 5              # 5
multiplicacion = 10 * 5     # 50
division = 10 / 5           # 2.0
potencia = 2 ** 3           # 8
```

### Trabajar con Listas
```python
colores = ["rojo", "azul", "verde"]
numeros = [1, 2, 3, 4, 5]
primero = colores[0]        # "rojo"
ultimos_dos = numeros[-2:]   # [4, 5]
```

### Bucles (Repetir acciones)
```python
for i in range(5):
    print(i)                # Imprime 0, 1, 2, 3, 4

for color in colores:
    print(color)            # Imprime cada color
```

### Funciones (Reutilizar código)
```python
def saludar(nombre):
    print(f"¡Hola, {nombre}!")

saludar("María")            # ¡Hola, María!
```

---

## 📊 Análisis de Datos con Pandas

### Cargar datos
```python
import pandas as pd
df = pd.read_csv('investigacion_datos.csv')
```

### Explorar datos
```python
df.head()               # Ver primeras filas
df.info()               # Información sobre columnas
df.describe()           # Estadísticas básicas
df.shape                # Dimensiones (filas, columnas)
```

### Operaciones comunes
```python
promedio = df['valor'].mean()           # Promedio
maximo = df['valor'].max()              # Valor máximo
minimo = df['valor'].min()              # Valor mínimo
total = df['valor'].sum()               # Suma total
```

### Filtrar datos
```python
tipo_a = df[df['categoria'] == 'TipoA']  # Filtrar por categoría
valores_altos = df[df['valor'] > 150]    # Filtrar por valor
```

---

## 🎓 Estructura de los Cuadernos

Cada cuaderno contiene:

| Elemento | Descripción |
|----------|-------------|
| **Títulos** | Organizan el contenido por temas |
| **Explicaciones** | Textos en español que explican conceptos |
| **Código** | Bloques de código que puedes ejecutar |
| **Resultados** | Salida del código (gráficos, tablas, etc.) |
| **Preguntas** | Desafíos para verificar tu comprensión |

### Cómo Usar los Cuadernos

1. **Lee** la explicación cuidadosamente
2. **Ejecuta** el código (presiona Shift + Enter o el botón ▶)
3. **Observa** los resultados
4. **Experimenta** modificando el código
5. **Resuelve** los ejercicios propuestos

---

## 🔧 Funcionalidades de Python Útiles

### Imprimir Información
```python
print("Este es un mensaje")
print(f"La edad es: {edad}")  # Usar variables dentro del texto
```

### Operaciones Condicionales
```python
if edad >= 18:
    print("Es un adulto")
elif edad >= 13:
    print("Es un adolescente")
else:
    print("Es un niño")
```

### Diccionarios
```python
persona = {
    'nombre': 'Carlos',
    'edad': 30,
    'ciudad': 'Madrid'
}
print(persona['nombre'])  # Carlos
```

---

## 📈 Ejemplo Práctico Completo

```python
# Paso 1: Cargar datos
import pandas as pd
df = pd.read_csv('investigacion_datos.csv')

# Paso 2: Explorar
print(f"El dataset tiene {df.shape[0]} filas y {df.shape[1]} columnas")
print(df.head())

# Paso 3: Analizar
promedio = df['valor'].mean()
print(f"Valor promedio: {promedio}")

# Paso 4: Filtrar
datos_tipo_a = df[df['categoria'] == 'TipoA']
print(f"Hay {len(datos_tipo_a)} datos de TipoA")

# Paso 5: Visualizar
import matplotlib.pyplot as plt
df.groupby('categoria')['valor'].mean().plot(kind='bar')
plt.title('Valor Promedio por Categoría')
plt.show()
```

---

## ❓ Preguntas Frecuentes

**P: ¿Es necesario tener experiencia en programación?**  
R: ¡No! Este módulo está diseñado desde cero para todos.

**P: ¿Cuánto tiempo tarda completar el módulo?**  
R: Aproximadamente 2-3 horas, dependiendo de tu ritmo.

**P: ¿Puedo reutilizar el código en mis proyectos?**  
R: ¡Claro! El código está disponible para que lo uses libremente.

**P: ¿Qué hago si no entiendo algo?**  
R: Revisa los ejemplos, ejecuta el código paso a paso y consulta los recursos.

**P: ¿Hay una forma de practicar más?**  
R: Sí, en los ejercicios encontrarás desafíos y los recursos incluyen enlaces útiles.

---

## 🎯 Flujo de Aprendizaje Recomendado

```
Inicio (00_inicio.ipynb)
    ↓
Leer ejemplos (01_ejemplos.ipynb)
    ↓
Ejecutar código de ejemplos
    ↓
Resolver ejercicios (02_ejercicios.ipynb)
    ↓
Experimentar con variaciones
    ↓
¡Completado! ✅
```

---

## 💻 Atajos Útiles en los Cuadernos

| Acción | Atajo |
|--------|-------|
| Ejecutar celda actual | Shift + Enter |
| Ejecutar todas las celdas | Ctrl + Shift + Enter |
| Insertar celda abajo | Alt + Enter |
| Eliminar celda | D + D |
| Cambiar a Markdown | M |
| Cambiar a Código | Y |

---

## 📝 Notas Importantes

- **Seguridad**: Los datos en este módulo son ficticios y seguros
- **Entorno**: Puedes trabajar offline una vez descargues los materiales
- **Progreso**: No hay calificación, ¡el objetivo es aprender!
- **Ritmo**: Trabaja a tu propio ritmo, no hay prisa

---

## 🤝 Comunidad y Apoyo

- Este módulo fue creado para más de 500 personas de diferentes disciplinas
- Puedes colaborar con otros participantes
- Comparte tus experiencias y aprendizajes
- Todos tenemos diferentes ritmos y enfoques - ¡eso está perfecto!

---

## 📞 Obtén Ayuda

Si tienes dudas:
1. Revisa los ejemplos en `01_ejemplos.ipynb`
2. Lee las explicaciones en las celdas Markdown
3. Consulta los recursos en la carpeta `recursos/`
4. Experimenta ejecutando el código con pequeños cambios

---

## ✨ Consejos para Aprovechar al Máximo

🎯 **Sé Activo**: No solo leas, ejecuta el código y experimenta  
📝 **Toma Notas**: Escribe lo que aprendas en tus propias palabras  
🔄 **Repite**: Si algo no es claro, vuelve a leerlo y ejecutarlo  
🧪 **Experimenta**: Modifica el código y observa qué pasa  
🎓 **Profundiza**: Una vez termines, busca desafíos adicionales  

---

## 📅 Estructura Temporal Sugerida

- **Semana 1**: Completa `00_inicio.ipynb` (30-45 minutos)
- **Semana 2**: Estudia `01_ejemplos.ipynb` (45-60 minutos)
- **Semana 3**: Resuelve `02_ejercicios.ipynb` (60-90 minutos)
- **Revisión**: Vuelve a repasar lo que más te interese

---

## 🎓 Después de Completar Este Módulo

Una vez termines, podrás:
- Aplicar Python a proyectos de tu propia disciplina
- Entender análisis de datos básicos
- Leer y modificar código de otros
- Continuar aprendiendo de forma independiente

---

## 📄 Licencia y Uso

Este material está disponible para fines educativos. Siéntete libre de usar, modificar y compartir según tus necesidades académicas.

---

**¡Bienvenido a tu viaje de aprendizaje!** 🚀  
Esperamos que disfrutes explorando el mundo de las herramientas de investigación.

---

*Última actualización: Septiembre 2026*  
*Para estudiantes de todas las disciplinas*
