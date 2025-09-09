# Proyecto: Generador de Material Educativo con Fast Prompting

Curso: IA — Generación de Prompts  
Autor: Camilo Gómez  

---

## Introducción
En el ámbito educativo, muchos docentes carecen de tiempo y recursos para generar material didáctico personalizado y atractivo. Esto impacta directamente en la motivación y el rendimiento de los estudiantes.

Problema: Falta de herramientas accesibles que permitan crear contenidos dinámicos, personalizados e interactivos sin necesidad de conocimientos técnicos avanzados.

Propuesta de solución:  
A través de técnicas de Fast Prompting, este proyecto permite generar:
- Cuestionarios de autoevaluación
- Resúmenes adaptados a diferentes niveles educativos
- Explicaciones paso a paso de temas complejos
- Prompts para ilustraciones educativas (usables en NightCafe u otras IAs generativas)

Viabilidad:  
- Uso de la API de Gemini (modelos gemini-1.5-flash y gemini-1.5-pro)  
- Recursos accesibles y costo optimizado gracias a prompts estructurados y reutilización de respuestas  
- Desarrollo acotado y aplicable en contextos reales de enseñanza  

---

## Objetivos
1. Aplicar técnicas de Fast Prompting para la generación de material educativo  
2. Desarrollar una Proof of Concept (POC) en Jupyter Notebook  
3. Minimizar las llamadas a la API y evaluar costos  
4. Explorar diferentes configuraciones de prompts y comparar resultados  
5. Analizar las mejoras logradas respecto a la propuesta inicial (Entrega 1)  

---

## Metodología
El desarrollo se llevó a cabo en las siguientes etapas:

1. Definición del problema basado en la necesidad de generar material educativo atractivo y accesible  
2. Diseño de prompts iniciales con ejemplos básicos (zero-shot)  
3. Optimización con Fast Prompting mediante role prompting, few-shot y prompts estructurados  
4. Comparación entre resultados de prompts simples y optimizados  
5. Implementación en Jupyter Notebook con funciones reutilizables para quiz, resúmenes, explicaciones e imágenes  
6. Evaluación de costos con pruebas en gemini-1.5-flash para iteraciones rápidas y gemini-1.5-pro para mayor calidad  

---

## Herramientas y Tecnologías
- Lenguaje: Python (Jupyter Notebook)  
- Modelos de IA: Gemini (gemini-1.5-flash y gemini-1.5-pro)  
- Librerías principales: google-generativeai, ipywidgets, dotenv  

Técnicas de Prompting utilizadas:  
- Zero-shot: generación directa sin ejemplos previos  
- Few-shot: prompts con ejemplos de salida esperada  
- Role prompting: instrucciones como “actúa como profesor de secundaria de biología”  
- Structured prompting: salida en JSON o Markdown para mayor claridad  

---

## Implementación
El código principal se encuentra en la notebook `entrega2_gomez.ipynb`.  

Funciones principales:  
- `quiz_prompt(topic)` genera cuestionarios de autoevaluación  
- `summary_prompt(topic)` crea resúmenes adaptados  
- `explanation_prompt(topic)` produce explicaciones paso a paso  
- `image_prompt(goal)` genera prompts para ilustraciones educativas  

Ejecución:  
1. Clonar este repositorio  
2. Instalar dependencias  
   ```bash
   pip install -r requirements.txt
