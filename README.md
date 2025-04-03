# RF-DETR: La Revolución en Computer Vision

## ¿Qué es RF-DETR?

RF-DETR (Robust Feature Detection Transformer) es un modelo de vanguardia en el campo de la visión por computador que combina la potencia de la arquitectura Transformer con técnicas avanzadas de extracción de características para lograr una detección de objetos precisa y eficiente.

A diferencia de los sistemas tradicionales de detección, RF-DETR utiliza mecanismos de atención para identificar y localizar objetos en imágenes y videos con una precisión sin precedentes, superando las limitaciones de los modelos CNN convencionales.

## Arquitectura Transformer y Rendimiento

RF-DETR aprovecha la arquitectura Transformer, originalmente diseñada para procesamiento de lenguaje natural, adaptándola perfectamente al dominio visual. Este enfoque permite:

- **Atención global sobre la imagen**: Captura relaciones de largo alcance entre diferentes regiones
- **Aprendizaje paralelo**: Procesamiento más eficiente que los modelos secuenciales
- **Representaciones ricas**: Características más robustas para la detección de objetos

### Benchmark COCO

En el dataset de referencia COCO (Common Objects in Context), RF-DETR ha demostrado resultados sobresalientes:

| Modelo | AP | AP50 | AP75 | APs | APm | APl |
|--------|-------|--------|--------|-------|-------|-------|
| RF-DETR Base | 45.3 | 63.1 | 49.8 | 28.5 | 49.2 | 61.7 |
| RF-DETR Large | 49.7 | 67.9 | 54.2 | 32.1 | 53.6 | 65.8 |

## Versiones Disponibles

RF-DETR está disponible en dos variantes principales:

- **RF-DETR Base**: Ideal para aplicaciones generales con un buen equilibrio entre rendimiento y recursos computacionales
- **RF-DETR Large**: Ofrece el máximo rendimiento para casos de uso que requieren la máxima precisión

## ¡Al Código!

### Instalación y Setup con Python

Para comenzar a utilizar RF-DETR, sigue estos pasos:

```bash
# Clonar el repositorio
git clone https://github.com/sandrarairan/rf-detr-computer-vision.git
cd rf-detr-computer-vision

# Crear y activar entorno virtual (opcional pero recomendado)
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# Instalar dependencias
pip install -r requirements.txt

# Descargar modelos pre-entrenados
python scripts/download_models.py
```

## Implementación por Etapas

### Etapa 1: Detección de Objetos en Imágenes

La primera etapa te permite detectar objetos en imágenes estáticas, sirviendo como fundamento para entender el funcionamiento del modelo.


### Etapa 2: Detección de Objetos en Video (Análisis Frame-by-Frame)

En esta etapa, extendemos la detección a videos, procesando cada frame individualmente.

### Etapa 3: ¡Detección en Tiempo Real con Webcam!

Ahora, llevamos el poder de RF-DETR a aplicaciones en tiempo real utilizando la webcam.

### Etapa 4: Tracking de Objetos Únicos (Guardando Recortes y JSON)

Esta etapa implementa seguimiento de objetos, permitiendo identificar y seguir instancias específicas a lo largo del tiempo.

### Etapa 5: Detección Selectiva, Prioridades y Estadísticas

En la etapa final, refinamos la detección para enfocarnos en clases específicas y generar estadísticas avanzadas.


