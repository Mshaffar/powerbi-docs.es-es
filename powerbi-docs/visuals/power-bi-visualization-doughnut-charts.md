---
title: Gráficos de anillos en Power BI
description: Gráficos de anillos en Power BI
author: mihart
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/05/2020
ms.author: rien
LocalizationGroup: Visualizations
ms.openlocfilehash: 2e2c108a5d05c7095526a813d33bed718f68f4c4
ms.sourcegitcommit: a199dda2ab50184ce25f7c9a01e7ada382a88d2c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2020
ms.locfileid: "82865354"
---
# <a name="create-and-use-doughnut-charts-in-power-bi"></a>Creación y uso de gráficos de anillos en Power BI

[!INCLUDE[consumer-appliesto-nyyn](../includes/consumer-appliesto-nyyn.md)]

[!INCLUDE [power-bi-visuals-desktop-banner](../includes/power-bi-visuals-desktop-banner.md)]

Un gráfico de anillos es similar a un gráfico circular porque muestra la relación de las partes con el todo. La única diferencia es que el centro está en blanco y deja espacio para un icono o una etiqueta.

## <a name="prerequisite"></a>Requisito previo

En este tutorial se usa el [archivo PBIX del Ejemplo de análisis de minoristas](https://download.microsoft.com/download/9/6/D/96DDC2FF-2568-491D-AAFA-AFDD6F763AE3/Retail%20Analysis%20Sample%20PBIX.pbix).

1. En la sección superior izquierda de la barra de menús, seleccione **Archivo** > **Abrir**.
   
2. Busque la copia del **archivo PBIX del Ejemplo de análisis de minoristas**.

1. Abra el **archivo PBIX del Ejemplo de análisis de minoristas** en la vista de informe ![Captura de pantalla del icono de vista de informe](media/power-bi-visualization-kpi/power-bi-report-view.png).

1. Seleccionar ![Captura de pantalla de la pestaña amarilla.](media/power-bi-visualization-kpi/power-bi-yellow-tab.png) para agregar una nueva página.


> [!NOTE]
> Para compartir el informe con un compañero en Power BI es necesario que los dos tengan licencias de Power BI Pro individuales o que el informe esté guardado en la capacidad Premium.    

## <a name="create-a-doughnut-chart"></a>Crear un gráfico de anillos

1. Empiece en una página de informe en blanco y, en el panel Campos, seleccione **Ventas** \> **Ventas del año anterior**.  
   
3. En el panel Visualizaciones, seleccione el icono del gráfico de anillos ![icono del gráfico de anillos](media/power-bi-visualization-doughnut-charts/power-bi-icon.png) para convertir el gráfico de barras en un gráfico de anillos. Si **Ventas del último año** no está en el área **Valores**, arrástrelo aquí.
     
   ![Panel de visualización con anillos seleccionados](media/power-bi-visualization-doughnut-charts/power-bi-doughnut-chart.png)

4. Seleccione **Elemento** \> **Categoría** para agregarlo al área **Leyenda**. 
     
    ![Anillos junto al panel Campos](media/power-bi-visualization-doughnut-charts/power-bi-doughnut-done.png)

5. Si lo desea, [ajuste el tamaño y el color del texto del gráfico](power-bi-visualization-customize-title-background-and-legend.md). 

## <a name="considerations-and-troubleshooting"></a>Consideraciones y solución de problemas
* La suma de los valores del gráfico de anillos debe ser el 100%.
* Demasiadas categorías dificultan la lectura y la interpretación.
* Los gráficos de anillos son útiles para comparar una sección determinada con el total, en lugar de comparar secciones individuales entre sí. 

## <a name="next-steps"></a>Pasos siguientes
[Gráficos de embudo en Power BI](power-bi-visualization-funnel-charts.md)

[Tipos de visualización en Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)


