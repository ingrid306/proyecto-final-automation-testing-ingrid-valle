Proyecto-final-automation-testing-ingrid-valle

Proposito del proyecto: realizar testeos de prueba automatizados en el sitio "https://www.saucedemo.com"


🧪 Proyecto de Automatización QA – UI & API (Python + Pytest + Selenium)

Este proyecto implementa un framework completo de automatización de pruebas UI y API utilizando Python, Pytest, Selenium WebDriver, y técnicas de Data-Driven Testing.
Incluye pruebas funcionales, validaciones de back-end con APIs, generación de reportes y una estructura modular basada en buenas prácticas de QA Automation.

📁 Estructura del Proyecto

project/
├── api/
│   ├── conftest.py
│   ├── test_cart_page.py
│   ├── test_checkout_complete_page.py
│   ├── test_checkout_page.py
│   ├── test_invetory_page.py
│   ├── test_login_page.py
│   └── test_reqres.py
│
├── data/
│   ├── __init__.py
│   ├── data-login.py
│   ├── data_login.csv
│   └── data_login.json
│
├── page/
│   ├── __init__.py
│   ├── cart_page.py
│   ├── checkout_page.py
│   ├── checkout_Complete_page.py
│   ├── inventory_page.py
│   └── login_page.py
│
├── reports/
│   ├── report_all.html
│   ├── report_api.html
│   └── report_ui.html
│
├── test/
│   ├── conftest.py
│   ├── test_cart_page.py
│   ├── test_checkout_page.py
│   ├── test_invetory_page.py
│   └── test_login_page.py
│
├── utils/
│   ├── __init__.py
│   ├── example_csv.py
│   ├── faker.py
│   └── helpers.py
│
└── README.md


🔧 Tecnologías Utilizadas

Python 3.x

Pytest

Selenium WebDriver

Requests (para pruebas API)

WebDriver Manager

Faker (generación de datos aleatorios)

CSV y JSON para Data Driven Testing

Pytest HTML para reportes

🎯 Objetivos del Proyecto

✔ Probar funcionalidades críticas de una aplicación web (UI)
✔ Probar APIs públicas (ReqRes)
✔ Implementar POM (Page Object Model)
✔ Parametrizar pruebas usando CSV y JSON
✔ Integrar Faker para datos dinámicos
✔ Generar reportes HTML separados por área (UI / API / All)
✔ Manejar fixtures desde conftest.py

🧱 Arquitectura del Framework
🔹 1. Page Object Model (POM)

Ubicada en /page/, contiene una clase por página:

login_page

inventory_page

cart_page

checkout_page

checkout_Complete_page

Cada clase incluye:

Localizadores

Acciones

Métricas de validación

🔹 2. Tests UI

En la carpeta /test/
Ejemplos cubiertos:

Login

Inventario

Carrito

Checkout

🔹 3. Tests API

En /api/ con Requests.
Incluye pruebas a:

ReqRes API

Simulaciones de endpoints del proyecto (cart, login, checkout)

🔹 4. Data Driven Testing

Los archivos en /data/ permiten ejecutar pruebas usando:

CSV

JSON

Python dicts

🔹 5. Utils

Herramientas auxiliares:

faker.py → datos ficticios

helpers.py → funciones comunes

example_csv.py → lector CSV

🔹 6. Reports HTML

La carpeta /reports/ contiene resultados automáticos:

report_ui.html

report_api.html

report_all.html
