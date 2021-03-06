---
title: Registro de cambios del servidor de informes de Power BI
description: Este registro de cambios es para el servidor de informes de Power BI y enumera los elementos nuevos junto con las correcciones de errores de cada versión publicada.
author: jtarquino
manager: kfile
ms.reviewer: maggies
ms.service: powerbi
ms.component: powerbi-report-server
ms.topic: conceptual
ms.date: 03/31/2018
ms.author: jtarquino
ms.openlocfilehash: ec97676fc043f9d8bd014465cc1fd2c0ffcca423
ms.sourcegitcommit: 52278d8e0c23ae5eaf46b10a6a2f1fb071a0f1cc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/16/2018
ms.locfileid: "40257151"
---
# <a name="changelog-for-power-bi-report-server"></a>Registro de cambios del servidor de informes de Power BI

Este registro de cambios es para el servidor de informes de Power BI y enumera los elementos nuevos junto con las correcciones de errores de cada versión publicada.

Para obtener información detallada sobre las nuevas características, consulte [Novedades en el servidor de informes de Power BI](whats-new.md). 

## <a name="august-2018"></a>Agosto de 2018
- **Servidor de informes de Power BI**
    - *Versión 1.3.6801.38816 (compilación 15.0.2.540), fecha de publicación: 15 de agosto de 2018*
        - Características
            - Compatibilidad de Direct Query de SSO de SAP HANA con Kerberos ya disponible para informes de Power BI
            - API de objeto visual personalizada incluida con la versión: versión 1.13.0
            - Los objetos visuales personalizados se revierten a una versión anterior compatible con la versión actual de la API de servidor (si está disponible)

- **Power BI Desktop (optimizado para Power BI Report Server)**
    - *Versión: 2.61.5192.64 (agosto de 2018), fecha de publicación: 15 de agosto de 2018*
        - Contiene los cambios necesarios para la conexión con Power BI Report Server (agosto de 2018)         
        
## <a name="march-2018"></a>Marzo de 2018
- **Servidor de informes de Power BI**
    - *Versión 1.2.6690.34729 (compilación 15.0.2.402), fecha de publicación: 27 de abril de 2018*
        - Correcciones de errores
            - Habilitar la migración de catálogos de SQL Server Reporting Services 2017
            - Para informes de Power BI (PBIX)
                - Los informes se pueden actualizar cuando un servidor está configurado para usar la autenticación personalizada
                - La modificación de las propiedades de un informe no restablece las credenciales del origen de datos
            - Para informes paginados (RDL)
                - El uso de `Lookup()` o de funciones derivadas, como `LookupSet()` y `MultiLookup()` en expresiones RDL ya no da como resultado `#Error`
                - Los informes vinculados respetan el tamaño de página del informe de destino al imprimir
                - Se pueden crear suscripciones para informes vinculados que usan parámetros en cascada
                - Los valores predeterminados de parámetros de varios valores pueden modificarse cuando se usa IE11
                - Se pueden editar las opciones de entrega de las suscripciones controladas por datos
                - Las suscripciones se pueden ver y editar mientras la suscripción se encuentra en ejecución
                - La definición de las credenciales del origen de datos no elimina las cadenas de conexión basadas en expresiones
            - Para los KPI
                - Las líneas de tendencia se actualizan cuando se actualizan los datos
            - Mejoras generales de la estabilidad

    - *Versión 1.2.6660.39920 (compilación 15.0.2.389), fecha de publicación: 28 de marzo de 2018*
        - Correcciones de errores
            - Para los informes de Power BI (PBIX), corrección para Exportar datos que no funcionan desde los objetos visuales de Power BI
            - Para los informes de Power BI (PBIX), corrección para los filtros de URL que no funcionan
            - Para los informes paginados (RDL), corrección para las imágenes que no se muestran correctamente en IE11 después de actualizar a la versión de marzo de Power BI Report Server

    - *Versión 1.2.6648.38132 (Build 15.0.2.378). Fecha de publicación: 19 de marzo de 2018*
        - Actualizaciones de seguridad
        - Mejoras de accesibilidad
        - Correcciones de errores
            - Para informes paginados (RDL), corrección de la visibilidad de los parámetros en un informe vinculado que se revierte después de editar sus propiedades
            - Corrección del portal web con autenticación de formularios personalizada que omite la cookie de expiración deslizante
            - Corrección para las exportaciones a Word que crean un alto de filas desigual si el contenido de la fila está vacío
            - Para informes paginados (RDL), corrección de la cadena de conexión basada en expresiones que se elimina cuando se cambia la credencial para el origen de datos
            - Corrección de la capacidad de usar KPI con valores de texto
            - Para informes paginados (RDL), corrección de la capacidad de asignar un nuevo conjunto de datos a un informe paginado existente (RDL)
            - Otras correcciones de estabilidad y facilidad de uso

- **Power BI Desktop (optimizado para Power BI Report Server)**
    - Versión: 2.56.5023.1043 (marzo de 2018). Fecha de publicación: 19 de marzo de 2018
        - Contiene los cambios necesarios para la conexión con Power BI Report Server (marzo de 2018)

## <a name="october-2017"></a>Octubre de 2017

- **Servidor de informes de Power BI**
    - *Versión 1.1.6582.41691 (compilación 14.0.600.442), fecha de publicación: 10 de enero de 2018*
        - Actualizaciones de seguridad
        - Correcciones de errores
            - Corrección del error que provocaba que GetParameters devolviese 400.
            - Corrección de la configuración de conjuntos de datos compartidos en informes paginados existentes (RDL).
            - Corrección de la excepción ExecutionNotFoundException al exportar informes con valores de parámetros distintos a PDF.

    - *Versión 1.1.6551.5155 (compilación 14.0.600.438), fecha de publicación: 11 de diciembre de 2017*
        - Correcciones de errores
            - Error al guardar los datos después de la actualización para determinados informes de Power BI Desktop.

    - *Versión 1.1.6530.30789 (compilación 14.0.600.437), fecha de publicación: 17 de noviembre de 2017*
        - Correcciones de errores
            - Corrección de los escenarios de autenticación básica 
            - Corrección del error por el que los días laborables no se podían seleccionar en la página de Suscripciones, Planes de actualización de caché e Instantáneas del historial en el Portal
            - En el caso de los informes paginados (RDL), corrección del error por el que, al tener expresiones en el cuadro de texto con la propiedad CanGrow establecida en false, los valores no muestran colores y las fuentes no son correctas
            - Para los informes de Power BI (PBIX), corrección del error por el que, al agregar leyendas al gráfico de líneas, se representa un objeto visual vacío

    - *Versión 1.1.6514.9163 (compilación 14.0.600.434), fecha de publicación: 1 de noviembre de 2017*
        - Correcciones de errores
            - Se han solucionado los problemas de confiabilidad de carga de los informes PBIX de más de 500 MB
            - Se ha corregido el problema de carga de datos de los informes PBIX de más de 1 GB

    - *Versión 1.1.6513.3500 (compilación 14.0.600.433), fecha de publicación: 31 de octubre de 2017*
        - Características
            - Compatibilidad con el modelo de datos insertados
            - Visualización de libros de Excel (con la integración de Office Online Server habilitada)
            - Actualización de datos programada (PBIX)
            - Compatibilidad con Direct Query
            - Compatibilidad con archivos de gran tamaño (hasta 2 GB)
            - API de REST pública
            - Compatibilidad con conjuntos de datos compartidos en Power BI Desktop (a través de oData)
            - Compatibilidad con parámetros de dirección URL para archivos PBIX
            - Mejoras de accesibilidad

- **Power BI Desktop (optimizado para Power BI Report Server)**
    - *Versión: 2.51.4885.3981 (octubre de 2017), fecha de publicación: 10 de abril de 2018*
        - Actualizaciones de seguridad

    - *Versión: 2.51.4885.2501 (octubre de 2017), fecha de publicación: 10 de enero de 2018*
        - Actualizaciones de seguridad

    - *Versión: 2.51.4885.1423 (octubre de 2017), publicado: 17 de noviembre de 2017*
        - Correcciones de errores
            - Corrección del error por el que Power BI Desktop de 32 bits no se puede ejecutar en sistemas operativos x86
            - Para los informes de Power BI (PBIX), corrección para mostrar las líneas de cuadrícula del eje X
            - Otras correcciones de errores menores

    - *Versión: 2.51.4885.1041 (octubre de 2017), publicado: 31 de octubre de 2017*
        - Características
            - Contiene los cambios necesarios para la conexión con Power BI Report Server (octubre de 2017)

## <a name="june-2017"></a>Junio de 2017

- **Servidor de informes de Power BI**
    - *Compilación 14.0.600.309, fecha de publicación: 10 de enero de 2018*
        - Actualizaciones de seguridad

    - *Compilación 14.0.600.305, publicado: 19 de septiembre de 2017*  
        - Correcciones de errores
            - Actualización a la versión más reciente del [control Web de mapas de Bing](https://msdn.microsoft.com/library/mt712542.aspx)

    - *Compilación 14.0.600.301, publicado: 11 de julio de 2017*
        - Correcciones de errores
            - La etiqueta `{{UserId}}` se resuelve en las credenciales almacenadas en lugar de ser el usuario el que ejecute el informe en los informes de Power BI
            - Algunas imágenes no se pueden representar en los informes del servidor de informes de Power BI
            - No se puede cambiar el nombre de un informe de Power BI en el servidor de informes de Power BI
            - No se pueden cargar los objetos visuales personalizados en la aplicación móvil de Power BI (es necesario volver a instalar la aplicación móvil para borrar la memoria caché local)

    - *Compilación 14.0.600.271, publicado: 12 de junio de 2017*
        - Versión inicial del servidor de informes de Power BI

- **Power BI Desktop (optimizado para Power BI Report Server)**
    - *Versión: 2.47.4766.4901 (junio de 2017), fecha de publicación: 10 de enero de 2018*
        - Actualizaciones de seguridad

## <a name="next-steps"></a>Pasos siguientes

[¿Qué es Power BI Report Server?](get-started.md)
[Información general de administrador](admin-handbook-overview.md)  
[Instalar un servidor de informes de Power BI](install-report-server.md)  
[Instalación del Generador de informes](https://docs.microsoft.com/sql/reporting-services/install-windows/install-report-builder)  
[Descargar SQL Server Data Tools (SSDT)](http://go.microsoft.com/fwlink/?LinkID=616714)

¿Tiene más preguntas? [Pruebe a preguntar a la comunidad de Power BI](https://community.powerbi.com/)
