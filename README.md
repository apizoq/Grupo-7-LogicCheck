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
\begin{center}
LogicCheck Lab quiere una herramienta educativa para mostrar cómo una computadora puede razonar sobre fórmulas proposicionales pequeñas. La idea no es de-
mostrar teoremas avanzados, sino hacer visible el proceso de asignar valores de verdad,

detectar contradicciones y retroceder.
Con pocas variables se puede hacer una tabla de verdad. Pero al aumentar el número de
variables, el espacio de combinaciones crece rápidamente. La clave es detectar temprano
cuando una cláusula ya no puede satisfacerse y evitar completar asignaciones inútiles.

Lo que deben construir. Un notebook que reciba fórmulas en forma de lista de cláu-
sulas, explore asignaciones de verdad con backtracking y determine si la fórmula es satis-
facible.
