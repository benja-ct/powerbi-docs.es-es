---
title: Conexión a Lithium con Power BI
description: Lithium para Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: maggiesMSFT
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 10/16/2017
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: 6cbd67a9c35726830fc862326d9a015b96952b83
ms.sourcegitcommit: fbb7924603f8915d07b5e6fc8f4d0c7f70c1a1e1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/02/2018
ms.locfileid: "37136304"
---
# <a name="connect-to-lithium-with-power-bi"></a>Conexión a Lithium con Power BI
Lithium entabla relaciones de confianza entre las mejores marcas del mundo y sus clientes, para ayudar a las personas a obtener respuestas y a compartir sus experiencias. Al conectar el paquete de contenido de Lithium a Power BI, puede medir las métricas clave sobre la comunidad en línea para contribuir a aumentar las ventas, reducir los costes de servicio y mejorar la lealtad. 

Conéctese al [paquete de contenido de Lithium](https://app.powerbi.com/getdata/services/lithium) para Power BI.

>[!NOTE]
>El paquete de contenido de Power BI usa la API de Lithium. Un exceso de llamadas a la API puede causar cargos adicionales de Lithium (consulte al administrador de Lithium).

## <a name="how-to-connect"></a>Cómo conectarse
1. Seleccione **Obtener datos** en la parte inferior del panel de navegación izquierdo.
   
   ![](media/service-connect-to-lithium/pbi_getdata.png) 
2. En el cuadro **Servicios** , seleccione **Obtener**.
   
   ![](media/service-connect-to-lithium/pbi_getservices.png) 
3. Seleccione **Lithium** \> **Obtener**.
   
   ![](media/service-connect-to-lithium/lithiumconnect.png)
4. Proporcione la dirección URL de la comunidad de Lithium. Tendrá el formato *https://community.yoursite.com*.
   
   ![](media/service-connect-to-lithium/params.png)
5. Cuando se le solicite, escriba sus credenciales de Lithium. Seleccione **oAuth 2** como el mecanismo de autenticación, haga clic en **Iniciar sesión** y siga el flujo de autenticación de Lithium.
   
   ![](media/service-connect-to-lithium/creds.png)
   
   ![](media/service-connect-to-lithium/creds2.png)
6. Una vez completado el flujo de inicio de sesión, se iniciará el proceso de importación. Cuando haya finalizado, aparecerá un nuevo panel, informes y modelo en el panel de navegación. Seleccione el panel para ver los datos importados.
   
    ![](media/service-connect-to-lithium/lithium.png)

**¿Qué más?**

* Pruebe a [hacer una pregunta en el cuadro de preguntas y respuestas](power-bi-q-and-a.md), en la parte superior del panel.
* [Cambie los iconos](service-dashboard-edit-tile.md) en el panel.
* [Seleccione un icono](service-dashboard-tiles.md) para abrir el informe subyacente.
* Aunque el conjunto de datos se programará para actualizarse diariamente, puede cambiar la programación de actualización o actualizarlo a petición mediante **Actualizar ahora**.

## <a name="system-requirements"></a>Requisitos del sistema
El paquete de contenido de Lithium requiere Lithium Community v15.9 o superior. Consulte al administrador de Lithium para confirmarlo.

## <a name="next-steps"></a>Pasos siguientes
[¿Qué es Power BI?](power-bi-overview.md)

[Power BI: Conceptos básicos](service-basic-concepts.md)

