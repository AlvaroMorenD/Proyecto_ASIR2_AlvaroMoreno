[Volver al índice general](../README.md)

# UD1 – Análisis del entorno y detección de necesidades tecnológicas

## Índice de apartados

- [ ] **1. Análisis del sector tecnológico**
- [ ] **2. Selección de la empresa o contexto de trabajo**
- [ ] **3. Identificación de necesidades tecnológicas**
- [ ] **4. Oportunidades y viabilidad del proyecto**
- [ ] **5. Obligaciones legales y normativas**
- [ ] **6. Guion inicial del proyecto**

## 1. Análisis del sector tecnológico

Para empezar, sevilla se ha convertido en el líder tecnológico de Andalucía, controlando el 40% de todo el sector TIC (Tecnologías de la Información) de la comunidad. Lo que antes llamábamos antes "la Cartuja" ahora se llama **Sevilla TechPark** y es donde están las grandes empresas del sector informático.

Hay una media de 31.667 personas trabajando en **Sevilla TechPark**. De todos ellos, casi 12.000 son informáticos o de telecomunicaciones. Las empresas de ingeniería dentro del parque han disparado su actividad un 73% este año.

Ahora si, pasamos al análisis de la infraestructura tecnológica sevillana;

Casi toda la provincia (el 99%) tiene acceso a internet básico, pero la clave está en la Fibra Óptica (FTTH) de alta velocidad. En la capital y el área metropolitana (como en el parque Sevilla TechPark), la velocidad es altísima porque las empresas lo necesitan para mover datos pesados.

Unos de los problemas es que muchas empresas por dentro tienen redes viejas (cables de cobre antiguos) que hacen cuello de botella. Por experiencia como becario en la Diputación de Sevilla. Nuestro trabajo como administrador de sistemas es cambiar esas redes viejas por redes modernas para que la velocidad real llegue al ordenador del trabajador.

En cuánto a las infraestructuras de las empresas, ya están aspostando por una infraestructura híbrida que mezcle el cloud con lo físico. Las empresas contratan Data Centers profesionales que les permite no depender de sus recursos. Las empresas guardan los datos secretos como por ejemplo las bases de datos, los documentos, etc... En su oficina (en un servidor local) y el resto (correo, webs) lo tienen en la nube de Amazon o Google. 

## 2. Selección de la empresa o contexto de trabajo

He seleccionado como entorno de trabajo la **Sociedad Provincial de Informática de Sevilla S.A.U. (INPRO)**. Se trata de una sociedad instrumental dependiente de la Diputación de Sevilla, que actúa como el principal proveedor tecnológico para las Entidades Locales de la provincia.

Este entorno, se dedica a gestionar la **Red TARSIS** que interconecta las sedes municipales, garantizando la seguridad perimetral y el acceso a internet. Además de desarrollar y mantiener el software necesario para el funcionamiento interno de los ayuntamientos, incluyendo sistemas de contabilidad, gestión de padrón, recursos humanos y gestión documental.
También, alojan los portales web corporativos de los municipios, así como los portales de Transparencia y Datos Abiertos.

En caso necesario, tienen un departamento de **atención a usuarios (CAU)** y **sistemas** para resolver incidencias tanto físicas como telemáticas, que garantizan que tanto el personal de diputación y distintos personales de ayuntamientos de sevilla, tengan disponibilidad a los distintos recursos tecnológicos que la entidad pone a su disposición para el desempeño de sus funciones.

<p align="center">
  <img src="img/tarsis.png_1186095565.png" alt="" width="600">
</p>

## 3. Identificación de necesidades tecnológicas

- Pese al acceso web seguro y al 2FA que oferecen para acceder de manera telemática a sus eqipos de trabajo, depender de PCs físicos con sistemas operativos obsoletos genera riesgos de fuga de información y dificultades de mantenimiento.

**Mi solución:** Implantar el **"Entorno Virtual Corporativo"** **(VDI)**. Usaremos la autenticación actual para servir escritorios virtuales centralizados en el CPD, garantizando que la información nunca salga del CPD y eliminando la gestión de parches en los equipos locales.

- La Seguridad en Municipios menores de 20.000 habitantes son el eslabón más débil y la mayoría no cumplen el Esquema Nacional de Seguridad (ENS) por falta de recursos.

**Mi Solución:** Desplegar un SOC Provincial (Centro de Operaciones de Seguridad) para monitorizar y proteger centralizadamente a todos los municipios, suprimiendo la falta de personal técnico.

- En cuanto a los **Silos de Información.** Existe la duplicidad y aislamiento de datos por la falta de comunicación entre departamentos.

**Mi Solución:** Implementar un **Bus de Interoperabilidad** sobre **SUSE Rancher**. Esto conecta las aplicaciones para lograr el "Dato Único", automatizando el intercambio de información y eliminando burocracia.

## 4. Oportunidades y viabilidad del proyecto

## Enlaces a recursos de la unidad 

- [Documentos de la unidad](./documentos/)
- [Diagramas e imágenes](./img/)

  ## Bibliografía / Webgrafía 
- Autor1, Título del libro o artículo, Editorial/Año.
- Sitio web oficial: [Enlace](https://www.ejemplo.com)
- Tutoriales y guías recomendadas: [Enlace](https://www.ejemplo2.com)



