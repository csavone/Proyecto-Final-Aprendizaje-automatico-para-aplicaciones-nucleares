# DETECCIÓN DE ANOMALÍAS EN EQUIPOS ROTANTES Proyecto-Final-Aprendizaje-automático-para-aplicaciones-nucleares

Objetivo: Detección de anomalías en máquinas rotantes
Datos: : 5000 registros de sensores de una máquina rotativa (vibración de ejes, temperatura, corriente eléctrica, velocidad de rotación (RPM) y presión interna, etc.). Cada registro tiene una etiqueta que indica el tipo de falla (sin falla, falla de rodamiento, desequilibrio del rotor, desalineación) y un indicador binario de requerimiento de mantenimiento (para cualquier tipo de falla).
Técnicas: se utilizarán algoritmos de aprendizaje no supervisado (sin etiquetas): PCA, K-means, DBSCAN. Solo se usarán las etiquetas para validación de resultados.
Con los primeros 3 componenetes principales pueden verse 2 grupos diferenciados
<img width="832" height="542" alt="image" src="https://github.com/user-attachments/assets/b1959efe-dff4-46e7-9d0d-ccab8c4f49cb" />

K-means para 2 clusters logra agrupar correctamente los patrones con y sin falla
<img width="353" height="279" alt="image" src="https://github.com/user-attachments/assets/98baea5e-3148-4f64-a332-c821312d7fb1" />

Definir centroide inicial para la clase sin falla permitió reconocer el cluster sin anomalías
<img width="894" height="631" alt="image" src="https://github.com/user-attachments/assets/dea73530-19f9-4747-81e2-1d5d03b28207" />
