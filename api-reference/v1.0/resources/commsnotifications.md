---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4c41a8657ebc144a7247a5e40984866c71d66154
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871000"
---
# <a name="commsnotifications-resource-type"></a>tipo de recurso commsNotifications

Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                                 | Descrição                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| valor          | coleção [commsNotification](commsnotification.md) | A notificação de uma alteração no recurso. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
