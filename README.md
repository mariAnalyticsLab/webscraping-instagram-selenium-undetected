# webscraping-instagram-selenium-undetected
### Web Scraping - Extracción de menciones, usuarios que comentaron, usuarios etiquetados por el usuario con Selenium en Instagram

## Descripción del algoritmo
Este proyecto implementa un script de web scraping utilizando Python, Selenium y `undetected_chromedriver` para extraer información de perfiles públicos de Instagram.
El algoritmo automatiza el inicio de sesión, la búsqueda de un perfil específico, la navegación por sus publicaciones y la recopilación de datos relacionados con comentarios, menciones, descripciones y usuarios etiquetados.

## Funcionamiento básico
El script realiza las siguientes acciones:

1. Inicia un navegador Chrome utilizando `undetected_chromedriver`.
2. Accede a Instagram e inicia sesión con credenciales proporcionadas por el usuario.
3. Busca un perfil específico.
4. Realiza scroll para obtener los enlaces de publicaciones (imágenes y reels).
5. Accede a cada publicación y extrae:
   - Usuarios que comentaron.
   - Comentarios de las publicaciones.
   - Menciones en comentarios y descripciones.
   - Usuarios etiquetados en publicaciones.
6. Limpia las menciones detectadas eliminando emojis y caracteres innecesarios.

## Resultados y aprendizajes obtenidos
A partir del desarrollo de este ejercicio se logró:
- Comprender el uso de Selenium para automatizar interacciones web.
- Aplicar técnicas de scroll dinámico para cargar contenido.
- Extraer información estructurada desde páginas con contenido dinámico.
- Manejar expresiones regulares para detectar menciones.
- Integrar librerías como `undetected_chromedriver` para reducir bloqueos.

## Herramientas y tecnologías utilizadas
- Python
- Selenium
- undetected-chromedriver
- BeautifulSoup
- pandas
- re

## Datos y archivos importantes
- Script principal en Python con la lógica de automatización y extracción.
- Variables generadas durante la ejecución:
  - Usuarios que comentaron.
  - Menciones detectadas.
  - Usuarios etiquetados.
  - Descripciones de publicaciones.

## Limitaciones
- El script depende de la estructura HTML actual de Instagram, la cual puede cambiar.
- Requiere credenciales válidas para iniciar sesión.
- No está optimizado para grandes volúmenes de perfiles.
- Su uso debe ser exclusivamente educativo y respetar los términos de servicio de la plataforma.
