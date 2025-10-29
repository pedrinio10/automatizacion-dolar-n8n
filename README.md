# 💸 Automatización del Dólar Diario con n8n

![Banner del proyecto](banner.png)

## 🧠 Descripción

Este flujo automatiza la consulta diaria de la cotización del **dólar estadounidense (USD)** frente al **peso argentino (ARS)** utilizando **n8n**.  
Obtiene los datos desde una API pública y envía un correo con la información actualizada mediante **Gmail**, con un diseño moderno en HTML.

---

## ⚙️ Flujo de trabajo

**Estructura general:**

[Cron] → [HTTP Request] → [Gmail]


- **Cron:** ejecuta el flujo automáticamente todos los días a una hora determinada.  
- **HTTP Request:** obtiene los datos de la API `https://open.er-api.com/v6/latest/USD`.  
- **Gmail:** envía un correo con la cotización actual del dólar.

---

## 🔧 Tecnologías utilizadas

- [n8n](https://n8n.io) – Plataforma de automatización sin código.  
- [Open ER API](https://open.er-api.com) – API gratuita de tipo REST para cotizaciones de divisas.  
- Gmail – Integración para el envío automático de correos.

---

## 🧩 Ejemplo de resultado

📩 **Asunto del correo:**  
> 💸 Cotización del Dólar Hoy  

📧 **Cuerpo del mensaje:**

> 💵 1 USD = **981.15 ARS** 🇦🇷  
> 📅 Actualizado el 27/10/2025  
>  
> *Automatizado por n8n 🚀*

---

## 🕓 Ejecución automática

El flujo está configurado para ejecutarse todos los días a las **09:00 AM**, aunque se puede modificar fácilmente desde el nodo **Cron**.

---

## 📁 Estructura del repositorio

📦 automatizacion-dolar-n8n
┣ 📜 dolar_automation.json # Flujo exportado desde n8n
┣ 🖼️ banner.png # Imagen del proyecto
┗ 📘 README.md # Documentación


---

## 🧑‍💻 Autor

**Pedro Pérez**  
🎓 Estudiante de Ingeniería en Sistemas – UTN Córdoba  
🔗 [LinkedIn](https://www.linkedin.com/in/pedro-perez-912716280/)  
🐙 [GitHub](https://github.com/pedrinio10)

---

## 🚀 Próximos pasos

- Agregar lógica condicional para comparar el valor con el día anterior y mostrar 📈 o 📉.  
- Integrar con Telegram o WhatsApp para recibir alertas instantáneas.  
- Publicar todos los flujos en un dashboard de automatizaciones personales.
