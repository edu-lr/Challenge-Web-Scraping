# Books to Scrape: ETL Completo

Este proyecto realiza un proceso ETL (Extracción, Transformación y Carga) para recolectar información de 1000 libros desde la web [books.toscrape.com](https://books.toscrape.com/).

## 🚀 ¿Qué hace el código?

1. **Scraping:** Extrae datos de 1000 libros distribuidos en 50 categorías (título, precio, rating, descripción, UPC).
2. **API (Open Library):** Consulta cada libro para encontrar a su autor, país, año de nacimiento y total de obras. Usa caché para optimizar el proceso.
3. **Base de Datos:** Guarda todo limpiamente en una base de datos **SQLite** (`libros.db`) estructurada en 4 tablas relacionales (`categorias`, `autores`, `libros`, `libro_autor`).

## ⚙️ Cómo usarlo

1. Clona el repositorio.
2. Instala los requerimientos: `pip install requests beautifulsoup4`
3. Abre y ejecuta las celdas de `esqueleto.ipynb`.

*(El script generará automáticamente un archivo de respaldo `libros_backup.json` y la base de datos `libros.db`).*
