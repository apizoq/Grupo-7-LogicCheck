# GRUPO-7
LogicCheck: un pequeño verificador de satisfacibilidad.
Universidad Nacional de Colombia — Sede Manizales  
Introducción a las Ciencias de la Computación  
Profesor: Carlos Manuel Orrego Franco  
Exposición: 19 de junio de 2026

--------

## Integrantes

| Nombre |
|--------|
| Alaham Daniel Aarón Daza |
| Andrés Fabricio Pizo  | 
| Mariana Zapata Fernández | 

------

## El problema
Proyecto 8. LogicCheck: un pequeño verificador de satisfacibilidad
LogicCheck Lab quiere una herramienta educativa para mostrar cómo una computadora puede razonar sobre fórmulas proposicionales pequeñas. La idea no es de-
mostrar teoremas avanzados, sino hacer visible el proceso de asignar valores de verdad, detectar contradicciones y retroceder.
Con pocas variables se puede hacer una tabla de verdad. Pero al aumentar el número de variables, el espacio de combinaciones crece rápidamente. La clave es
detectar temprano cuando una cláusula ya no puede satisfacerse y evitar completar asignaciones inútiles.

Lo que deben construir. Un notebook que reciba fórmulas en forma de lista de cláu-
sulas, explore asignaciones de verdad con backtracking y determine si la fórmula es satis-
facible.

## Cómo ejecutar en Google Colab

1. Abrir [Google Colab](https://colab.research.google.com)
2. Ir a **Archivo → Abrir notebook → GitHub**
3. Pegar la URL del repositorio: `https://github.com/apizoq/Grupo-7-LogicCheck.git`
4. Seleccionar `Notebook de Google Colab-GRUPO 7.ipynb`
5. Ejecutar todo: **Runtime → Run all**

## Qué hace el algoritmo
El algoritmo LogicCheck funciona como un detective inteligente que busca una combinación correcta de respuestas (Verdadero o Falso) para las variables de una fórmula, usando una estrategia llamada Backtracking (Búsqueda con Retroceso).
1.Prueba con orden: El algoritmo le da un valor (True o False) a una variable a la vez, avanzando como si recorriera un árbol de decisiones.

2.Poda (Ahorra tiempo): Después de cada paso, revisa las reglas. Si ve que una regla ya se rompió y es imposible de arreglar, corta (poda) ese camino de inmediato para no perder tiempo explorándolo.

3.Retrocede (Backtrack): Al darse cuenta de que ese camino no tiene salida, da un paso atrás, borra su última decisión e intenta con la otra opción
