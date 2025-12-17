# Componentes de una Aplicación de IA

Microsoft estructura las aplicaciones de Inteligencia Artificial en cuatro capas fundamentales, proporcionando soporte y servicios específicos para cada etapa del desarrollo.

## 1. Capa de Datos (Data Layer)
Es la base estructural de la aplicación. Se encarga de la recopilación, almacenamiento y administración de la información para entrenamiento, inferencia y toma de decisiones.

* **Tipos de Datos:**
    * **Estructurados:** Bases de datos tradicionales (ej. Azure SQL, PostgreSQL).
    * **No estructurados:** Documentos, imágenes, archivos multimedia.
    * **Tiempo real:** Flujos de datos continuos.
* **Servicios Clave:** Azure Cosmos DB, Azure Data Lake.
* **Concepto PaaS (Plataforma como Servicio):** Microsoft ofrece bases de datos gestionadas donde el usuario no administra la infraestructura (hardware/SO), situándose en un punto medio entre IaaS y SaaS.

## 2. Capa de Modelo (Model Layer)
Abarca la selección, entrenamiento e implementación de los modelos de ML e IA. Incluye herramientas para ajustar (*fine-tuning*), evaluar y versionar modelos.

* **Tipos de Modelos:**
    * **Preentrenados:** Listos para usar (ej. Azure OpenAI en Foundry Models).
    * **Personalizados:** Creados desde cero (ej. Azure Machine Learning).
* **Microsoft Foundry:** PaaS unificada para operaciones de IA empresarial que ofrece un catálogo completo de modelos.

## 3. Capa de Cómputo (Compute Layer)
Proporciona los recursos de procesamiento necesarios para entrenar y ejecutar los modelos.

| Servicio | Descripción y Uso |
| :--- | :--- |
| **Azure App Service** | Hospedaje de aplicaciones web y APIs. |
| **Azure Functions** | Ejecución *serverless* (sin servidor) controlada por eventos. |
| **Azure Container Instances (ACI)** | Ejecución ligera de contenedores. Ideal para implementación rápida y escalado sencillo. |
| **Azure Kubernetes Service (AKS)** | Orquestación de contenedores a nivel empresarial (Kubernetes totalmente administrado). |

> **Nota:** Las **API** (Interfaces de Programación de Aplicaciones) son esenciales en esta capa, ya que definen cómo se comunican los componentes de software de forma segura.

## 4. Capa de Integración y Orquestación
Conecta los modelos y los datos con la lógica de negocio y las interfaces de usuario finales.

**El papel de Microsoft Foundry:**
Actúa como pieza clave ofreciendo:
* **Servicio de Agentes:** Para crear agentes inteligentes que razonan y actúan.
* **Herramientas de IA:** Acceso a APIs de voz, visión y lenguaje.
* **SDKs y APIs:** Kits de desarrollo para integrar funcionalidades.
* **Gestión:** Herramientas de portal para administrar modelos y flujos de trabajo.

*El objetivo es insertar la inteligencia directamente dentro de la capa de datos para crear aplicaciones más capaces.*