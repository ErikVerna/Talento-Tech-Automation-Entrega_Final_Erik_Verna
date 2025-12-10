# Proyecto de Talento Tech

## Proposito del proyecto
Este proyecto tiene como objetivo automatizar pruebas de UI y de API para el sitio **SauceDemo**, aplicando practicas como Page Object Model, manejo de datos externos, generacion de reportes HTML, logging y captura automatica de pantalla.

## Tecnologias utilizadas
- Python 3.x
- Pytest
- Selenium WebDriver
- Logging
- Faker
- CSV / JSON
- Request

## 📑 Estructura del proyecto

- **assets/** → Recursos gráficos y estáticos utilizados en reportes.
- **datos/** → Archivos de entrada y datos de prueba.
- **logs/** → Registros de ejecución y trazabilidad de procesos.
- **pages/** → Páginas o plantillas relacionadas con la automatización.
- **reports/** → Reportes generados automáticamente.
- **tests/** → Casos de prueba automatizados.
- **utils/** → Funciones auxiliares y herramientas de soporte.
- **conftest.py** → Configuración de Pytest.
- **run_tests.py** → Script principal para ejecutar pruebas.
- **report.html** → Ejemplo de reporte generado.
- **readme.md** → Documento de referencia del proyecto.

## Reportes y Logs

El proyecto genera tres tipos principales de resultados durante la ejecucion de las prubas: **reporte HTML**, **capturas de pantalla**, **archivo de log**

### Reporte HTML
Se genera un reporte HTML detallado con el nombre de ```reporte.hmtl``` en la **carpeta raiz** del proyecto

### Logs de ejecución
Tambien se genera un log con informacion detallada de toda la ejecución de las pruebas en la siguiente ubicacion: ```logs/suite.log```

### Capturas de pantalla

Se realizan capturas de pantalla por cada test que haya fallado y se encuentran en la siguiente ubicacion: ```reports/screens/```

## Ejuctar todas las pruebas
Para iniciar la ejecucion de las pruebas debes ejecutar la siguiente linea:

```bash
python -m run_test.py
```

## ¿Como interpretar los reportes?
- Al ejecutar `run_test.py`, se genera un archivo HTML en la carpeta raiz.
- El reporte incluye:
    - Lista completa de test ejecutados
    - El estado de cada prueba
    - La duracion de cada test
    - Las capturas de pantalla para pruebas fallidas

## Pruebas incluidas
- Login exitoso y fallido
- Login exitoso y fallido usando faker
- Comportamiento de la pagina de inventario
- Comportamiento de la pagina del carrito
- API (Reqres): GET users, POST create user, DELETE user, validaciones de codigos HTTP, validaciones de estructura JSON

## Manejo de datos de prueba
- En la carpeta `datos` se incluyen archivos como:
    - `data_login.csv` -> datos de usuarios validos o invalidos
    - `productos.json` -> datos de productos para validacion

## Autor
SggSeguridad  Alias: Rockito
- Referente institucional y especialista técnico en seguridad informática, automatización y monitoreo IP.
- Este proyecto forma parte de la línea de trabajo orientada a la mejora continua, trazabilidad y documentación técnica.

### Conclusion
Este proyecto ofrece una estructura organizada y escalable para automatizar pruebas de API utilizando Python y Pytest. Incluye un flujo simple de ejeucion mediante `run_test.py`, generacion automatica de reporte HTML facilitando el analisis de las pruebas.

La arquitectura del proyecto esta pensada para agregar nuevos casos de prueba y configuraciones sin modificar el nucleo del proyecto, manteniendo buenas practicas y permitiendo su escalabilidad en el tiempo.


# 🚀 Proyecto de Talento Tech – Automatización de Pruebas

## 🎯 Propósito del Proyecto
El objetivo de este proyecto es automatizar pruebas **UI** y **API** sobre el sitio **SauceDemo**, aplicando buenas prácticas de automatización como **Page Object Model (POM)**, manejo de datos externos, generación automática de reportes HTML, logging estructurado y capturas de pantalla ante fallos.

---

## 🛠️ Tecnologías Utilizadas
- **Python 3.x**
- **Pytest**
- **Selenium WebDriver**
- **Logging**
- **Faker**
- **CSV / JSON**
- **Requests**

---

## 📂 Estructura del Proyecto

assets/ → Recursos gráficos usados en reportes
datos/ → Datos de entrada para pruebas (CSV/JSON)
logs/ → Registros de ejecución
pages/ → Implementación del Page Object Model
reports/ → Reportes generados automáticamente
tests/ → Casos de prueba UI y API
utils/ → Funciones auxiliares
conftest.py → Configuración de Pytest
run_tests.py→ Script principal para ejecutar pruebas
report.html → Ejemplo de reporte generado
readme.md → Documentación del proyecto


---

## 📝 Reportes y Logs

### 📄 Reporte HTML
- Se genera automáticamente con el nombre **`reporte.html`** en la **carpeta raíz**.
- Incluye:
  - Estado de cada prueba  
  - Tiempos de ejecución  
  - Capturas de pantalla asociadas a errores  

### 🧾 Logs de Ejecución
- Archivo generado: **`logs/suite.log`**
- Contiene:
  - Flujo de ejecución  
  - Errores  
  - Información contextual para depuración  

### 📸 Capturas de Pantalla
- Se guardan únicamente cuando un test falla  
- Ubicación: **`reports/screens/`**

---

## ▶️ Ejecución de las Pruebas
Para ejecutar la suite completa:

```bash
python -m run_test.py
```

🧪 Pruebas Incluidas

🔐 UI – Login

Login exitoso

Login fallido

Login utilizando datos generados con Faker

🛒 UI – Funcionalidades Principales

Validación de la página de inventario

Pruebas sobre el carrito de compras

🌐 API – Reqres

GET users

POST create user

DELETE user

Validación de códigos HTTP

Validación de estructura JSON

📊 Manejo de Datos de Prueba

Ubicados dentro de datos/:

data_login.csv → Usuarios válidos e inválidos

productos.json → Información para validaciones de productos

👤 Autor

Erik Tomas Verna
Analista en Sistemas
Enfoque en automatización, calidad de software y documentación técnica.

✔️ Conclusión

Este proyecto proporciona una arquitectura clara, ordenada y fácilmente escalable para automatizar pruebas con Python y Pytest. Su diseño permite agregar nuevos casos y configuraciones sin modificar el núcleo del sistema, asegurando mantenibilidad, trazabilidad y eficiencia a largo plazo.