---
title: Utilice un filtro o una segmentación de fecha relativa en Power BI Desktop
description: Obtenga información acerca de cómo usar un filtro o una segmentación de datos para restringir los intervalos de fechas relativas en Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 07/27/2018
ms.author: davidi
LocalizationGroup: Create reports
ms.openlocfilehash: 4168bc6bfcab72a6be58a7616aeed2c19bce3205
ms.sourcegitcommit: f01a88e583889bd77b712f11da4a379c88a22b76
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/27/2018
ms.locfileid: "39329027"
---
# <a name="use-a-relative-date-slicer-and-filter-in-power-bi-desktop"></a>Uso de un filtro o una segmentación de fecha relativa en Power BI Desktop
Con la **segmentación de fecha relativa** o el **filtro de fechas relativas**, puede aplicar filtros basados en el tiempo a cualquier columna de fecha del modelo de datos. Por ejemplo, puede usar la **segmentación de fecha relativa** para mostrar solo los datos de las ventas realizadas en los últimos treinta días (o mes, meses naturales, etc). Y, al actualizar los datos, el período de tiempo relativo aplica automáticamente la restricción de fecha relativa correspondiente.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_01.png)

## <a name="using-the-relative-date-range-slicer"></a>Uso de una segmentación de intervalo de fecha relativa
Puede usar la segmentación de fecha relativa igual que cualquier otra segmentación. Solo tiene que crear un objeto visual de **segmentación** para el informe y luego seleccionar un valor de fecha para el valor **Campo**. En la siguiente imagen, se ha seleccionado el campo *OrderDate*.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_02.png)

Seleccione el acento circunflejo en la esquina superior derecha de la **segmentación de fecha numérica** y aparecerá un menú.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_03.png)

Para la segmentación de fecha relativa, seleccione *Relativa*.

Después, puede seleccionar la configuración. En la primera lista desplegable de la *segmentación de fecha relativa*, tiene las siguientes opciones:

* Últimos
* Siguiente
* Este

Estas selecciones se muestran en la siguiente imagen.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_04.png)

La siguiente opción de configuración (central) en la *segmentación de fecha relativa* permite escribir un número para definir el intervalo de fechas relativas.

La tercera opción de configuración le permite elegir la medida de la fecha. Tiene las opciones siguientes:

* Días
* Semanas
* Semanas (calendario)
* Meses
* Meses (calendario)
* Años
* Años (calendario)

Estas selecciones se muestran en la siguiente imagen.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_05.png)

Si selecciona *Meses* en esa lista, y escribe 2 en la opción de configuración central, podría ocurrir lo siguiente: si hoy es 20 de julio, los datos incluidos en los objetos visuales restringidos por la segmentación mostrarían los datos de los dos meses anteriores, a partir del 20 de mayo hasta el 20 de julio (fecha de hoy).

En cambio, si seleccionó *Meses (calendario)*, los objetos visuales restringidos mostrarían los datos desde el 1 de mayo hasta el 30 de junio (los dos últimos meses naturales completos).

## <a name="using-the-relative-date-range-filter"></a>Uso de un filtro de intervalo de fecha relativa
También puede crear un filtro de intervalo de fecha relativa para la página del informe o el informe completo. Para ello, solo tiene que arrastrar un campo a las áreas **Filtros de nivel de página** o los **Filtros de nivel de informe**, en el panel **Campo**, como se muestra en la siguiente imagen.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_06.png)

Una vez allí, puede modificar el intervalo de fecha relativa de forma similar a como se personaliza la **segmentación de datos de fecha relativa**. Seleccione **Filtrado de fecha relativa** en la lista desplegable **Tipo de filtro**.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_07.png)

Después de seleccionar **Filtrado de fecha relativa**, verá tres secciones para modificar, incluido un cuadro numérico intermedio, igual que la segmentación.

![](media/desktop-slicer-filter-date-range/relative-date-range-slicer-filter_08.png)

Y eso es todo para utilizar estas restricciones de fecha relativa en los informes.

## <a name="limitations-and-considerations"></a>Limitaciones y consideraciones
Las siguientes limitaciones y consideraciones se aplican actualmente al filtro y la **segmentación de fecha relativa**.

* Los modelos de datos de **Power BI** no incluyen información de zona horaria. Los modelos pueden almacenar horas, pero no hay ninguna indicación de la zona horaria en la que se encuentran.
* El filtro y la segmentación siempre se basan en la hora UTC, por lo que si configura un filtro en un informe y enviarlo a un compañero de trabajo en una zona horaria diferente, ambos verán los mismos datos. Sin embargo, si no está en la zona horaria UTC, podría ver los datos correspondientes de una zona horaria diferente de la esperada.
* Los datos capturados en una zona horaria local se pueden convertir a UTC mediante el **Editor de consultas**.

