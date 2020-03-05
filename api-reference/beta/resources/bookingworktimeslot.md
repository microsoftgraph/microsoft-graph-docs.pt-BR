---
title: tipo de recurso bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2c9caa1f5a9a2b78911e77df27b84079efd70ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507877"
---
# <a name="bookingworktimeslot-resource-type"></a>tipo de recurso bookingWorkTimeSlot

Namespace: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
As horas de início e de término do trabalho.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end|TimeOfDay|A hora do dia em que o trabalho é iniciado. Por exemplo, 08:00:00.0000000.|
|iniciar|TimeOfDay|A hora do dia em que o trabalho é interrompido. Por exemplo, 17:00:00.0000000.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
