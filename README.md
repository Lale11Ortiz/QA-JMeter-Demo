# QA-JMeter-Demo

Proyecto de práctica de pruebas de performance utilizando Apache JMeter.
Se realiza una simulación de 10 usuarios concurrentes accediendo al endpoint `/posts` de la API pública JSONPlaceholder.
Incluye reporte HTML, estructura de carpetas ordenada y ejecución desde consola.

---

## 📌 Descripción técnica

- 🔧 Herramienta: Apache JMeter 5.6.3
- 🌐 API: https://jsonplaceholder.typicode.com/posts
- 👥 Usuarios simulados: 10
- 🔁 Ciclos por usuario: 1
- ⏱️ Ramp-Up: 5 segundos
- 📈 Reporte generado: Sí, en formato HTML

---

## 📁 Estructura del proyecto

QA-JMeter-Demo/
  - test-plan.jmx # Plan de pruebas JMeter
  - evidences/ # Resultados .jtl y capturas
  - report/ # Reporte HTML generado automáticamente
  - README.md (ESP)
  - README_En.md (ENG)

---

## ▶️ Cómo ejecutar el test desde consola

```bash
jmeter -n -t test-plan.jmx -l evidences/results.jtl -e -o report/

---

## 📊 Resultados del test

Total requests:     10
Duración:           6 segundos
Requests/segundo:   1.8
Tiempo promedio:    545 ms
Error rate:         0.00%