---
title: tipo de recurso de commsNotifications
description: Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83a89e848d0992d253efb532ed078031b6f965d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946298"
---
# <a name="commsnotifications-resource-type"></a>tipo de recurso de commsNotifications

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Lista de notificações usado pelos servidores Communications para envio de notificações de vários em um único lote.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                                 | Descrição                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| valor          | coleção [commsNotification](commsnotification.md) | A notificação de alteração no recurso. |

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
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
