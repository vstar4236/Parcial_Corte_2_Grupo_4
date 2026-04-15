# ☕ Solución Parcial Corte 2: Inteligencia de Negocios - Cafetería U. Sabana

**Nombres:** Matías Mondragón Osorio  - Arianne Amorocho - Mariana Peña Rodriguez
**Asignatura:** Programación y Decisiones  
**Fecha:** 15 de abril de 2026

## 🚀 Paso a Paso de la Solución

1. **Generación de Datasets:** Se crearon 3 archivos `.csv` originales ("sucios") con la información base de Clientes, Proveedores y Productos proporcionada en el parcial.
2. **Procesamiento con Pandas:** - Se aplicaron técnicas de normalización (1NF, 2NF, 3NF).
   - Se separaron columnas compuestas (`cliente_info`, `empresa_ciudad`, `producto_info`) para garantizar atomicidad.
   - Se gestionaron valores nulos (`NaN`) y se estandarizaron textos a formato Título/Capitalizado.
   - Se exportaron los datos limpios a nuevos archivos `.csv`.
3. **Migración SQLite:** - Se creó la base de datos `parcial_2_cafeteria.db`.
   - Se habilitó `PRAGMA foreign_keys = ON` para asegurar la integridad referencial.
   - Se cargaron los DataFrames procesados como tablas SQL.
4. **Arquitectura POO:** Se implementó una clase controladora para gestionar las operaciones CRUD (Create, Read, Update, Delete) y la generación de reportes mediante `JOIN`.

## 📁 Archivos en el Repositorio
* `clientes_sucios.csv`, `proveedores_sucios.csv`, `productos_sucios.csv`: Datos originales.
* `clientes_limpios.csv`, `proveedores_limpios.csv`, `productos_limpios.csv`: Datos procesados por Pandas.
* `parcial_2_cafeteria.db`: Base de Datos relacional final.
* `main.py`: Código fuente con la lógica completa.
