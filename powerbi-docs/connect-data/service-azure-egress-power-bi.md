---
title: Salida de Power BI y Azure
description: Obtención de información acerca de los cargos de salida de Azure y Power BI en función de la ubicación del inquilino y Power BI Premium
author: davidiseminger
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 05/08/2019
ms.author: davidi
LocalizationGroup: Data from databases
ms.openlocfilehash: b39812eb155d1d1c32ddba984986e5260f4b1ad1
ms.sourcegitcommit: 0e9e211082eca7fd939803e0cd9c6b114af2f90a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2020
ms.locfileid: "83302239"
---
# <a name="power-bi-and-azure-egress"></a>Salida de Power BI y Azure

Cuando se usa Power BI con orígenes de datos de Azure, puede evitar los cargos de salida de Azure asegurándose de que su inquilino de Power BI está en la misma región que los orígenes de datos de Azure.

Cuando el inquilino de Power BI se implementa en la misma región de Azure en la que se implementan los orígenes de datos, no se incurre en cargos de salida para la actualización programada y las interacciones de DirectQuery. 

## <a name="determining-where-your-power-bi-tenant-is-located"></a>Determinación de dónde se encuentra el inquilino de Power BI

Para averiguar dónde se encuentra el inquilino de Power BI, consulte el artículo [¿Dónde se encuentra mi inquilino de Power BI?](../admin/service-admin-where-is-my-tenant-located.md).

Para los clientes de Multi-Geo de Power BI Premium, si el inquilino de Power BI no está en la ubicación óptima para algunos de los orígenes de datos basados en Azure, se puede implementar las capacidades de Multi-Geo de Power BI Premium en la región de Azure deseada y beneficiarse de tener el inquilino de Power BI y los orígenes de datos de Azure en la misma región de Azure.

## <a name="next-steps"></a>Pasos siguientes

Para obtener más información acerca de Power BI Premium o Multi-Geo, eche un vistazo a los siguientes recursos:

* [¿Qué es Microsoft Power BI Premium?](../admin/service-premium-what-is.md)
* [Adquisición de Power BI Premium](../admin/service-admin-premium-purchase.md)
* [Compatibilidad con Multi-Geo en Power BI Premium (versión preliminar)](../admin/service-admin-premium-multi-geo.md)
* [¿Dónde se encuentra mi inquilino de Power BI?](../admin/service-admin-where-is-my-tenant-located.md)
* [Preguntas más frecuentes sobre Power BI Premium](../admin/service-premium-faq.md)
