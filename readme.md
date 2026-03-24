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

Erik Tomas Verna ~ Analista en Sistemas

✔️ Conclusión

Este proyecto proporciona una arquitectura clara, ordenada y fácilmente escalable para automatizar pruebas con Python y Pytest. Su diseño permite agregar nuevos casos y configuraciones sin modificar el núcleo del sistema, asegurando mantenibilidad, trazabilidad y eficiencia a largo plazo.
