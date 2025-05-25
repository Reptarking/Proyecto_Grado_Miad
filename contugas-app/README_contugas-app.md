# Contugas-App

Este módulo contiene el código del sistema web desarrollado para el proyecto de grado **Detección de Anomalías en Consumo de Gas**, como parte del curso MIAD 2025.

Incluye la aplicación Flask para mostrar KPIs, dashboards, realizar consultas, evaluar nuevas lecturas y exponer el modelo MLP+lags en tiempo real.

---

## 📂 Estructura de la carpeta

```
/contugas-app
├── app.py               # Aplicación principal Flask
├── requirements.txt     # Lista de dependencias Python
├── /templates           # Plantillas HTML (dashboard, consulta, alertas, evalua)
├── /static/css          # Archivos de estilo CSS
├── /data               # Dataset procesado con flag de anomalías
└── /venv (opcional)    # Entorno virtual (no incluir en entrega final)
```

---

## 🛠 Requisitos

- Python 3.8+  
- Recomendable usar entorno virtual (`venv`)  
- Power BI Service (para integración del iframe)

---

## ⚙ Instalación

1️⃣ Clonar el repositorio:
```bash
git clone [URL del repositorio]
cd contugas-app
```

2️⃣ Crear entorno virtual:
```bash
python -m venv venv
source venv/bin/activate   # En Linux/macOS
venv\Scripts\activate    # En Windows
```

3️⃣ Instalar dependencias:
```bash
pip install -r requirements.txt
```

---

## ▶ Ejecución

Lanzar la app Flask:
```bash
python app.py
```

Por defecto se ejecutará en `http://127.0.0.1:5000`

---

## 📌 Funcionalidades principales

✅ Dashboard general con KPIs  
✅ Consulta filtrada por cliente, fecha, anomalías  
✅ Visualización gráfica de serie temporal  
✅ Panel de evaluación de nuevas lecturas con modelo MLP+lags  
✅ Exportación de datos filtrados a CSV  
✅ Integración embebida con dashboard Power BI

---

## ⚠ Notas

- Asegúrate de tener el archivo `consolidated_data_con_anomalias.csv` en la carpeta `/data`  
- Si necesitas cambiar el puerto o modo de ejecución, ajusta las líneas finales de `app.py`

---

¡Listo para ejecución y pruebas locales!
