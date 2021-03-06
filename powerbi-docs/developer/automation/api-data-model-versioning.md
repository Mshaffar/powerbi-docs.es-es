---
title: Control de versiones de modelos de datos de Power BI
description: Modelo de datos expuesto por un servicio OData Service
author: KesemSharabi
ms.author: kesharab
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-developer
ms.topic: conceptual
ms.date: 06/08/2018
ms.openlocfilehash: 76947b1e311bbd1a21e09ce39461a70bed61d926
ms.sourcegitcommit: 7aa0136f93f88516f97ddd8031ccac5d07863b92
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/05/2020
ms.locfileid: "79079609"
---
# <a name="data-model-versioning"></a>Control de versiones de modelo de datos

El modelo de datos expuesto por un servicio OData, como el modelo de datos de Power BI, define un contrato entre el servicio de OData y sus clientes. Los servicios pueden ampliar su modelo siempre y cuando no interrumpan a los clientes existentes. Los cambios de última hora, como quitar propiedades o cambiar el tipo de las propiedades existentes, requieren que se proporcione una nueva versión de servicio en una dirección URL raíz de servicio diferente para el nuevo modelo.  
  
Las siguientes adiciones de modelo de datos se consideran seguras y no requieren servicios para controlar la versión de su punto de entrada.  
  
* Agregar una propiedad que acepta valores NULL o tiene un valor predeterminado; si tiene el mismo nombre que una propiedad dinámica existente, debe tener el mismo tipo (o el tipo base) como propiedad dinámica existente  
* Agregar una propiedad de navegación que acepta valores NULL o tiene un valor de colección; si tiene el mismo nombre que una propiedad de navegación dinámica existente, debe tener el mismo tipo (o el tipo base) como propiedad de navegación dinámica existente  
* Agregar un nuevo tipo de entidad al modelo  
* Agregar un nuevo tipo complejo al modelo  
* Agregar un nuevo conjunto de entidades  
* Agregar un nuevo valor singleton  
* Agregar una acción, una función, una importación de acciones o una importación de funciones
* Agregar un parámetro de acción que acepta valores NULL  
* Agregar una definición de tipo o enumeración  
* Agregar cualquier anotación a un elemento de modelo que el cliente no necesita comprender para interactuar correctamente con el servicio  
  
Los clientes ***DEBEN*** estar preparados para que los servicios realicen estos cambios incrementales en su modelo. En concreto, los clientes deben estar preparados para recibir las propiedades y los tipos derivados no definidos previamente por el servicio.  
  
Los servicios ***NO DEBEN*** cambiar su modelo de datos en función del usuario autenticado. Si el modelo de datos depende del usuario o del grupo de usuarios, todos los cambios deben ser seguros según la definición incluida en esta sección al comparar el modelo completo con el modelo visible para los usuarios con autorizaciones limitadas.  
  
Para más información sobre los estándares del modelo de datos OData, consulte [OData Version 4.0 Part 1: Protocol Plus Errata 02 (Versión de OData 4.0, parte 1: Protocol Plus Errata 02)](https://docs.oasis-open.org/odata/odata/v4.0/odata-v4.0-part1-protocol.html).  
  
## <a name="see-also"></a>Consulte también
[Información general sobre la API de REST de Power BI](https://docs.microsoft.com/rest/api/power-bi/)