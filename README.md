✈️ Data Sky — Customer Analytics

Autora: Samai Manuz Rodríguez
Lema: Volando con datos ☁️📊
Notebook principal: Examen Samai.ipynb

🎯 Objetivo

Analizar el comportamiento de los clientes de una aerolínea y evaluar si existen diferencias significativas en los vuelos reservados (Flights Booked) según el nivel educativo (Education), combinando EDA, limpieza y estadística inferencial.

🔧 Qué incluye el proyecto (resumen)

📥 Ingesta & unión de: actividad de vuelo + historial de fidelidad.

📈 EDA & Visualizaciones: distribución de reservas, relación de métricas y segmentaciones clave.

🧹 Limpieza mínima: deduplicados por Loyalty Number, normalización y tipificación.

🩹 Imputación dirigida:

Salary → mediana (robusta a outliers).

Cancellation Year/Month → 0 (alta ausencia; se recomienda evaluar su eliminación).

📊 Descriptivo por educación: count, mean, median, std de Flights Booked.

🧪 Pruebas de hipótesis: elección automática entre Student/Welch o Mann–Whitney según normalidad y varianzas (con post-hoc cuando aplica).

▶️ Uso rápido

Abre Examen Samai.ipynb.

Ejecuta las celdas en orden para reproducir limpieza, EDA y contrastes.

Revisa las tablas finales (descriptivas, IC 95%) y las conclusiones del contraste.

📁 Estructura elemental del proyecto:
.
├─ Examen Samai.ipynb            # Notebook contenedor de todo el proceso
├─ Full Customer Fixed.parquet   # Dataset final (inicialmente creado/guardado como csv)
├─ Descriptive Stats.parquet     # Tabla resumen por Education
├─ Hipótesis 1.parquet           # Resultado de la primera prueba de hipótesis ('Hight School or Below' -VS- 'Doctor')
└─ README.md                     # Descriptivo del proyecto

✅ Resultado

Un pipeline claro y reproducible que deja un dataset consolidado y evidencia estadística sobre las diferencias (o no), entre los diferentes subconjuntos de datos, listo para más pruebas de hipótesis y listo para la toma de decisiones.
