---
title: Acerca del ABCD
permalink: /docs/es/
lang: es
key: docs-quick-start-es
---

ABCD es un acrónimo para designar un conjunto de herramientas para la **A**utomatización de **B**ibliotecas y **C**entros de **D**ocumentación. Este acrónimo se mantiene en francés: **A**utomation des **B**ibliothèques et **C**entres de **D**ocumentacion y en portugués: **A**utomatização das **B**ibliotecas e dos **C**entros de **D**ocumentação. Aún en otros lenguajes no-latinos con variaciones leves pero aceptables, por ejemplo, en holandés: **A**utomatisering van **B**ibliotheken en **C**entra voor **D**ocumentatie, donde el acrónimo también se mantiene.

El nombre en si mismo expresa la ambición del producto: no solo proveer funciones de automatización para la bibliotecas 'clásicas', sino también para otros proveedores de información tales como los centros de documentación. Flexibilidad y versatilidad son los primeros criterios bajo los cuales el software ha sido desarrollado. Esta flexibilidad se ilustra, por ejemplo, en el hecho de que, en principio, prácticamente cualquier estructura bibliográfica puede ser manejada por el software. Del mismo modo, estructuras no-bibliográficas pueden ser creadas siempre y cuando la información sea mayormente 'textual', siendo ésta una limitación que emerge de la tecnología de base de datos que sirve de base al software, la cual es la base de datos textual (CDS/)ISIS. Una buena comprensión de algunos conceptos y técnicas básicas relacionadas con el ISIS, por ejemplo, el Lenguaje de Formateo, es crucial para el manejo experto del software ABCD. Por esta razón muchas secciones de la documentación también tratan de la tecnolocía ISIS subyacente.

ABCD se denomina una 'suite' de software para bibliotecas y centros de documentación porque está formado por módulos relativamente independientes, que pueden cooperar entre si, pero también pueden existir de manera aislada. De hecho, De hecho softwares avanzados ya existentes, que han mostrado su potencial en entornos exigentes como son las aplicaciones de BIREME (dentro del contexto de la Biblioteca Virtual en Salud), han sido adoptados y adaptados en ABCD - y esta es la razón por la cual sus nombres originales, tales como iAH, SeCS (ambas desarrolladas por Bireme) y EmpWeb (Empréstimos en Web) desarrollada origibalmente por KALIO ltda. del Uruguay y ampliamente probada en Chile) se mantienen. Estos componentes principales se muestran, con sus relaciones jerárquicas, en el segundo nivel, en la siguiente gráfica y a continuación son explicadas brevemente:

![Slide2](https://user-images.githubusercontent.com/20482054/137317883-75797ad3-47d5-43f0-b3b7-7c405f646236.JPG)

## ABCD Central

El componente **Central** de ABCD contempla modulos para Administración de Bases de Datos (creación de bases de datos, edición de las estructuras, utilitarios), Catalogación, Adquisiciones, Circulación/Préstamos y Estadísticas. También se está preparando un módulo de Gestión de Tesauros como parte del módulo de catalogación, para una base de datos específica con estructura de tesauro con control consistente de los niveles jerárquicos. Como parte de este módulo **central** podemos también mencionar servicios de importación y exportación, impresión y herramientas para la administración de la base de datos tales como bloqueo/desbloqueo y la realización de cambios globales sobre los campos de los registros. Si los (nuevos) módulos de 'Suministro de Documentos' y 'Biblioteca Digital' están instalados, el bibliotecólogo o admiministrador del sistema puede también proporcionar respuestas a las solicitudes de información y documentos digitales. De hecho, cualquier base de datos puede ser completamente administrada (edición, búsqueda, presentación ...) a partir de este 'hub' central. Este módulo 'Central', de hecho, representa el componente 'back-office' de ABCD, los usuarios no tienen acceso a él pero los resultados que ven y se les ofrece están totalmente definidos en este módulo central del software !


Cualquier estructura de base de datos ISIS puede ser definida y manejada en ABCD, con registros cuya longitud actual es de 1MB con un máximo de 4Gb para el tamaño de la base de datos (pero estas restricciones resultarán obsoletas en la próxima generación basada en NBP de ISIS y ABCD). En comparación con la tecnología ISIS 'normal', se usan claves de indización de 60 caracteres, (en lugar de las claves de 30 caracteres) lo que dá una mayor fortaleza en el control de listas de autoridades y tesauros a través de la definición de formatos de validación muy flexibles al momento de la entrada de datos. Toda la interacción está basada en tecnología WWW permitiendo, por ejemplo, cadenas de caracteres codificados en HTML para el ingreso a texto completo, indización, hiperenlaces a páginas de ayuda, etc. Es perfectamente posible automatizar completamente todas las funciones necesarias de una biblioteca pequeña, con muchos usuarios internos, usando únicamente el módulo 'Central', por cuanto la opción de búsqueda avanzada está ya incorporada, de modo tal que toda la funcionalidad está cubierta con un mínimo de complejidad tecnológica (solo ISIS y PHP).


## El OPAC de ABCD (iAH)


The public search interface (OPAC) is an adapted version of BIREME's general 'advanced interface for Health information' (iAH). It has all the 'classic' elements of online database searching through either a very simple 'Google'-like interface or more advanced ways of searching with field-selectors and Boolean operators. The iAH interface developed by BIREME is currently being upgraded to iAHx, ensuring it will align perfectly with modern Information Retrieval concepts and techniques (e.g. clustering, relevance ranking based on Lucene indexing). the ABCD Site


The search function is offered as part of an 'end-users' portal page, presenting the own catalog(s) in a much wider information context by providing access to other information resource.s (e.g. Google, Medline...) and communication (announcements, alerts), also paving the way for 'Web 2.0'-like functions. It allows meta-searches on not only the local catalogs but also many other information resources. A link to the dedicated OPAC's for each resource is also available.


El Administrador del Sitio actualmente es un Sistema Manejador de Contenidos específico, el cual permite diseñar la estructura y componentes del las páginas del portal de ABCD.


## El Sistema de Control de Publicaciones Seriadas (SeCS) de ABCD

This module offers an advanced management tool for serials/journals (classical and/or electronic) of any publication type (referring to periodicity). Serials as such but also issues of a serial and all types of publication patterns can be managed by this module. BIREME uses this technology e.g. for its products 'Portal of Scientific Journals' (see : http://portal.revistas.bvs.br/main.php?home=true&lang=en) and SCAD (see : http://scad.bvs.br/php/index.php?lang=en) which is the Brazilian union catalog of over 12.000 journals (with millions of issues) of more than 50 libraries.


## El Sistema de Préstamos Avanzado (EmpWeb) de ABCD

Este módulo ofrece un manejo avanzado de los préstamos con algunas opciones y características orientadas a organizaciones de mayor tamaño y complejidad. Provee una función 'MyLibrary' para los usuarios finales, a través del OPAC basada en tecnología 'web-services'. Puede utilizarse para reemplazar el módulo de préstamos que viene integrado en ABCD en caso que se necesite cumplir con las necesidades de políticas múltiples para préstamo así como situaciones de alto volúmen de transacciones.

------

La idea de una 'suite' refleja el hecho de que ABCD tiene partes relativamente independientes, al igual que en el caso de la suite de automatización de office (ej. Open Office, Microsoft Office) - pero con vinculaciones obvias de cooperación. Por ejemplo, el módulo de Estadísticas, un componente del módulo de Circulación y Préstamos, puede trabajar con cualquier base de datos ISIS, mientras que el IAH-OPAC también ofrece procedimientos de recuperación de información, basados en la tecnología web, sobre cualquier conjunto de bases de datos ISIS, no sólo las mantenidas bajo ABCD. El sistema de Control de Publicaciones Seriadas (SeCS) maneja bases de datos ISIS para seriadas dentro o fuera del contexto de ABCD. Pero creemos que juntas esas partes constituyen una 'suite' de herramientas muy poderosa y, como sistema integrado esperamos que 'el todo represente más que la suma de las partes' !