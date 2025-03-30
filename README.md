# Hackathon Sistecredito 4ta Versión 2025

## Integrantes
> Pablo García

> Tomás Lopera

> Pedro Sierra

## Descripción del Proyecto

**Problema:**  
> El objetivo de este reto es desarrollar un asistente virtual de inteligencia artificial que ayude a los clientes a negociar compromisos de pago ajustados a su situación financiera.

**Nuestra Solución:**  
> Implementación de un Agente Multiusos mediante OpenAI

## Pipeline del código CHATBOT

**Carga de librerías y configuración de API:**

> Se instala y configura la API de OpenAI.

> Se importan librerías como pandas, numpy y openai.

**Carga de plantillas de conversación:**

> Se define un diccionario llamado plantillas1 que contiene respuestas tipo (templates) para distintas situaciones (ej. prejuridico, administrativo, negociacion_cuotas, etc).

**Embeddings de plantillas:**

> Se genera un embedding para cada plantilla usando el modelo text-embedding-ada-002.

> Estos embeddings se almacenan en una lista como base de referencia.

**Carga del dataset:**

> Se sube un archivo CSV llamado negociaciones_chatbot (5).csv con columnas como Mensajes Cliente y Mensajes Agente.

**Detección de tipo de plantilla:**

> Se calcula el embedding de un mensaje nuevo del cliente.

> Luego se compara con los embeddings de las plantillas usando similitud del coseno.

> Se selecciona la plantilla más similar como respuesta adecuada.

## Tecnologías utilizadas

- **Python**
- **Pandas**
- **Matplotlib**
- **Open AI**
- **Gradio**

## Instalación y configuración

### Clonar repositorio
```bash
git clone https://github.com/Tomaslopera/Hackathon_Sistecredito.git
```

### Instalar dependencias
```bash
pip install pandas matplotlib seaborn openai gradio
```
