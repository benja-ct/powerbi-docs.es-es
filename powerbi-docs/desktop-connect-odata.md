---
title: Conectarse a una fuente OData en Power BI Desktop
description: Puede conectarse a una fuente OData en Power BI Desktop y usarla fácilmente
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 07/27/2018
ms.author: davidi
LocalizationGroup: Connect to data
ms.openlocfilehash: c84ef0f57398bd9573488c1a8c5b16fd5511dd87
ms.sourcegitcommit: f01a88e583889bd77b712f11da4a379c88a22b76
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/27/2018
ms.locfileid: "39328980"
---
# <a name="connect-to-odata-feeds-in-power-bi-desktop"></a>Conectarse a fuentes OData en Power BI Desktop
En Power BI Desktop, puede conectarse a una **fuente OData** y usar los datos subyacentes igual que cualquier otro origen de datos en Power BI Desktop.

Para conectarse a una fuente OData, seleccione **Obtener datos > Fuente OData** en la cinta **Inicio** en Power BI Desktop.

![](media/desktop-connect-odata/connect-to-odata_1.png)

En la ventana **Fuente OData** que aparece, escriba o pegue la URL de la fuente OData en el cuadro y seleccione **Aceptar**.

![](media/desktop-connect-odata/connect-to-odata_2.png)

Power BI Desktop se conecta a la fuente OData y muestra las tablas disponibles y otros elementos de datos en la ventana **Navegador**. Al seleccionar un elemento, el panel derecho de la ventana **Navegador** muestra una vista previa de los datos. Puede seleccionar tantas tablas como quiera importar. La ventana **Navegador** muestra una vista previa de la tabla seleccionada actualmente.

![](media/desktop-connect-odata/connect-to-odata_3.png)

Puede elegir el botón **Editar**, que inicia el **Editor de consultas**, donde puede dar forma y transformar los datos de la fuente OData antes de importarla en Power BI Desktop. O puede seleccionar el botón **Cargar** e importar todos los elementos de datos que ha seleccionado en el panel izquierdo.

Al seleccionar **Cargar**, Power BI Desktop importa los elementos seleccionados y muestra la ventana **Carga** del progreso de la importación.

![](media/desktop-connect-odata/connect-to-odata_4.png)

Una vez que haya finalizado, Power BI Desktop hace que las tablas seleccionadas y otros elementos de datos estén disponibles en el panel **Campos**, que se encuentra en el lado derecho de la vista *Informes* en Power BI Desktop.

![](media/desktop-connect-odata/connect-to-odata_5.png)

¡Eso es todo!

Ahora está preparado para usar los datos importados de la fuente OData en Power BI Desktop para crear objetos visuales, informes, o para interactuar con cualquier otro dato con el que quiera conectarse e importar, como otros libros de Excel, bases de datos o cualquier otro origen de datos.

### <a name="next-steps"></a>Pasos siguientes
Hay todo tipo de datos a los que puede conectarse con Power BI Desktop. Para obtener más información sobre orígenes de datos, consulte los siguientes recursos:

* [¿Qué es Power BI Desktop?](desktop-what-is-desktop.md)
* [Orígenes de datos en Power BI Desktop](desktop-data-sources.md)
* [Combinar datos y darles forma con Power BI Desktop](desktop-shape-and-combine-data.md)
* [Connect to Excel workbooks in Power BI Desktop (Conectarse a libros de Excel en Power BI Desktop)](desktop-connect-excel.md)   
* [Especificar datos directamente en Power BI Desktop](desktop-enter-data-directly-into-desktop.md)   

