---
title: Notificaciones de interrupción del servicio
description: Obtenga información sobre cómo recibir notificaciones por correo electrónico cuando se produzca una interrupción o degradación del servicio Power BI.
author: kfollis
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 05/11/2020
ms.author: kfollis
ms.openlocfilehash: 344ce3b83bbb9922e0359e04e65c01a1a088bcb3
ms.sourcegitcommit: bfc2baf862aade6873501566f13c744efdd146f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2020
ms.locfileid: "83135428"
---
# <a name="service-interruption-notifications"></a>Notificaciones de interrupción del servicio

Es fundamental tener información sobre la disponibilidad de las aplicaciones empresariales críticas. Power BI proporciona una notificación de incidentes para que pueda recibir mensajes de correo electrónico si se produce una interrupción o degradación del servicio. Aunque el Acuerdo de Nivel de Servicio (SLA) del 99,9 % de Power BI hace que estas repeticiones sean poco frecuentes, queremos asegurarnos de que esté informado. En la captura de pantalla siguiente se muestra el tipo de correo electrónico que recibirá si habilita las notificaciones:

![Correo electrónico de notificación de actualización](media/service-interruption-notifications/refresh-notification-email.png)

En este momento, se envían mensajes de correo electrónico para los siguientes _escenarios de confiabilidad_:

- Confiabilidad de apertura del informe
- Confiabilidad de actualización del modelo
- Confiabilidad de actualización de consultas

Las notificaciones se envían cuando se produce un _retraso prolongado_ en las operaciones (por ejemplo, al abrir un informe, al actualizar conjuntos de datos o al ejecutar consultas). Una vez que se ha resuelto un incidente, recibirá un correo electrónico de seguimiento.

> [!NOTE]
> En la actualidad, esta característica solo está disponible para capacidades dedicadas en Power BI Premium. No está disponible para la capacidad compartida o insertada.

## <a name="capacity-and-reliability-notifications"></a>Notificaciones de capacidad y fiabilidad

Cuando una capacidad de Power BI Premium está experimentando periodos largos de uso elevado de recursos que pueden afectar a la fiabilidad, se envía un correo electrónico de notificación. Entre los ejemplos de estos efectos se incluyen retrasos prolongados en operaciones como, por ejemplo, abrir un informe, actualización del conjunto de datos y ejecuciones de consultas. 

El correo electrónico de notificación proporciona información sobre el motivo del uso elevado de recursos, incluida la siguiente:

* Id. del conjunto de datos del responsable
* Tipo de operación
* Tiempo de CPU asociado al uso elevado de recursos

Power BI también envía notificaciones por correo electrónico cuando se detecta una sobrecarga en una capacidad de Power BI Premium. El correo electrónico explica el motivo más probable de la sobrecarga, las operaciones que han generado la carga en los 10 minutos anteriores y la carga de cada operación generada. 


Si tiene más de una capacidad Premium, el correo electrónico incluye información sobre esas capacidades durante el periodo sobrecargado, de este modo puede considerar la posibilidad de trasladar las áreas de trabajo que contengan elementos de uso intensivo de recursos a capacidades con la carga mínima.

Las notificaciones correos electrónicos de sobrecarga solo se envían cuando se desencadena un umbral de sobrecarga. Una vez que la carga de la capacidad Premium vuelva a los niveles no sobrecargados no recibirá un segundo correo electrónico.

En la imagen siguiente se muestra un ejemplo de correo electrónico de notificación:

![correo electrónico de notificación de capacidad sobrecargada](media/service-interruption-notifications/refresh-notification-email-2.png)


## <a name="enable-notifications"></a>Habilitación de notificaciones

Un administrador de inquilinos de Power BI habilita las notificaciones en el portal de administración:

1. Identifique o cree un grupo de seguridad habilitado para correo electrónico que deba recibir notificaciones.

1. En el portal de administración, seleccione **Configuración de inquilinos**. En **Configuración de ayuda y soporte técnico**, expanda **Recepción de notificaciones por correo electrónico sobre interrupciones o incidentes en el servicio**.

1. Habilite las notificaciones, escriba un grupo de seguridad y seleccione **Aplicar**.

    ![Habilitación de notificaciones del servicio](media/service-interruption-notifications/enable-notifications.png)

> [!NOTE]
> Power BI envía notificaciones desde la cuenta no-reply-powerbi@microsoft.com. Asegúrese de que esta cuenta esté en la lista de permitidas para que las notificaciones no terminen en una carpeta de correo no deseado.

## <a name="next-steps"></a>Pasos siguientes

[Opciones de soporte técnico de Power BI Pro y Power BI Premium](service-support-options.md)

¿Tiene más preguntas? [Pruebe la comunidad de Power BI](https://community.powerbi.com/)
