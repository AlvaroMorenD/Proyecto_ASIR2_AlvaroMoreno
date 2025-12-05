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

He seleccionado como entorno de trabajo la **Sociedad Provincial de Informática de Sevilla S.A.U. (INPRO)**. Se trata de una sociedad instrumental dependiente de la Diputación de Sevilla, con sede central en la capital hispalense, que actúa como el principal proveedor tecnológico para las Entidades Locales de la provincia.

Este entorno, se dedica a gestionar la **Red TARSIS** que interconecta las sedes municipales, garantizando la seguridad perimetral y el acceso a internet. Además de desarrollar y mantiener el software necesario para el funcionamiento interno de los ayuntamientos, incluyendo sistemas de contabilidad, gestión de padrón, recursos humanos y gestión documental.

También, alojan los portales web corporativos de los municipios, así como los portales de Transparencia y Datos Abiertos, fomentando la participación ciudadana.

En caso necesario, tienen un departamento de **atención a usuarios (CAU)** y **sistemas** para resolver incidencias tanto físicas como telemáticas, que garantizan que tanto el personal de diputación y distintos personales de ayuntamientos de sevilla, tengan disponibilidad a los distintos recursos tecnológicos que la entidad pone a su disposición para el desempeño de sus funciones.

![Red TARSIS](img/tarsis.png_1186095565.png)

## 3. Identificación de necesidades tecnológicas

Basándome en la documentación oficial del Plan Estratégico Provincial, he encontrado una serie de vulnerabilidades que pueden comprometer la seguridad y la continuidad de los servicios públicos;

- Dispone de sistemas de **copias de seguridad primarios**, se ha identificado la inexistencia de un **Centro de Proceso de Datos de backups secundario** que permita una conmutación efectiva en caso de desastre y que se pueda utilizar como espejo de datos.

**Solución:** Con **Proxmox Backup Server** podemos implementar un sistema de backups que se sincronize y actúe como espejo de datos con el primero. Y además la podemos implementar en la nube con **Amazon web service**, para que en caso que destrucción del CPD de basckups físico, el secundario no pueda ser destruido. **OpenSource y fácil de integrar**

- Existe una urgencia en la **"adecuación al Esquema Nacional de Seguridad (ENS)"**, especialmente en los ayuntamientos de menos de 20.000 habitantes. Los hackers saben que los pueblos pequeños son fáciles de atacar (tienen seguridad débil) y algunos no tienen dinero ni informáticos para mejorar la seguridad.

**Solución:** Desplegar una arquitectura de **firewalls** y segmentación de redes **VLANs** para aislar tráficos críticos, cumpliendo con las medidas de nivel medio/alto del **ENS** 

- El análisis **DAFO** de la documentación, identifica la existencia de **"silos en la gestión del dato"**, lo que provoca duplicidad de información y falta de comunicación entre los sistemas municipales.

**Solución:** implementar una arquitectura centralizada de datos y usuarios que elimine la duplicidad y garantice una fuente única de verdad para todos los departamentos. Implementaria **Active Directory** en **Windows** o **LDAP** en
**Linux**.

![CPD Diputación de Sevilla](img/tarsis.png_1186095565.png)

## 4. Oportunidades y viabilidad del proyecto

## Enlaces a recursos de la unidad 

- [Documentos de la unidad](./documentos/)
- [Diagramas e imágenes](./img/)

  ## Bibliografía / Webgrafía 
- Autor1, Título del libro o artículo, Editorial/Año.
- Sitio web oficial: [Enlace](https://www.ejemplo.com)
- Tutoriales y guías recomendadas: [Enlace](https://www.ejemplo2.com)

