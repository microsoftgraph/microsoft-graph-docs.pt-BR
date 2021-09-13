---
title: Tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de Comunicações para o envio de várias notificações em um único lote.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9bec8adec8f673f504fe2a907cef146c077d2fc7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084626"
---
# <a name="commsnotifications-resource-type"></a>Tipo de recurso commsNotifications

Namespace: microsoft.graph

Lista de notificações usadas pelos servidores de Comunicações para o envio de várias notificações em um único lote.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                                 | Descrição                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| valor          | [Coleção commsNotification](commsnotification.md) | A notificação de uma alteração no recurso. |

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

