---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9e77c95c4303e02be7ac6ef91caf02e9c2d3ce6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531794"
---
# <a name="commsnotifications-resource-type"></a>tipo de recurso commsNotifications

Namespace: microsoft.graph

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
