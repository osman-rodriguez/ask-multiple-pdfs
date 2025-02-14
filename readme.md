# MultiPDF Chat App

utilice este video apra hacerlo [YouTube](https://youtu.be/dXxQ0LR-3Hg). aunque modifique varias cositas..

## Introducción
# ----------------------------
# La aplicación MultiPDF Chat es una aplicación en Python que te permite chatear con múltiples documentos PDF. 
# Puedes hacer preguntas sobre los PDFs utilizando lenguaje natural, y la aplicación proporcionará respuestas 
# relevantes basadas en el contenido de los documentos. 
# Esta app utiliza un modelo de lenguaje para generar respuestas precisas a tus consultas. 
# Ten en cuenta que la aplicación solo responderá preguntas relacionadas con los PDFs cargados.

## Cómo Funciona
# ----------------------------

# [Diagrama de la aplicación MultiPDF Chat](./docs/PDF-LangChain.jpg)

# La aplicación sigue estos pasos para proporcionar respuestas a tus preguntas:

# 1. Carga de PDFs: La aplicación lee múltiples documentos PDF y extrae su contenido en texto.

# 2. Segmentación del texto: El texto extraído se divide en fragmentos más pequeños para procesarlos de manera eficiente.

# 3. Modelo de lenguaje: La aplicación utiliza un modelo de lenguaje para generar representaciones vectoriales 
#    (embeddings) de los fragmentos de texto.

# 4. Coincidencia por similitud: Cuando haces una pregunta, la aplicación la compara con los fragmentos de texto 
#    y encuentra los más similares semánticamente.

# 5. Generación de respuesta: Los fragmentos seleccionados se pasan al modelo de lenguaje, que genera una respuesta 
#    basada en el contenido relevante de los PDFs.

## Dependencias e Instalación
# ----------------------------
# Para instalar la aplicación MultiPDF Chat, sigue estos pasos:

# 1. Clona el repositorio en tu máquina local.

# 2. Instala las dependencias requeridas ejecutando el siguiente comando:
pip install -r requirements.txt

# 3. Obtén una clave API de OpenAI y agrégala al archivo `.env` en el directorio del proyecto:
echo "OPENAI_API_KEY=tu_clave_secreta_api" >> .env

## Uso
# ----------------------------
# Para usar la aplicación MultiPDF Chat, sigue estos pasos:

# 1. Asegúrate de haber instalado las dependencias necesarias y de haber agregado la clave API de OpenAI en el archivo `.env`.

# 2. Ejecuta el archivo `main.py` usando el CLI de Streamlit. Ejecuta el siguiente comando:
streamlit run app.py

# 3. La aplicación se abrirá en tu navegador web predeterminado, mostrando la interfaz de usuario.

# 4. Carga múltiples documentos PDF en la aplicación siguiendo las instrucciones proporcionadas.

# 5. Haz preguntas en lenguaje natural sobre los PDFs cargados utilizando la interfaz de chat.


