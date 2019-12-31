---
title: tipo de recurso commsNotification
description: Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05a800d4732ae54dd6c8b1ce76074b64625b9c16
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913356"
---
# <a name="commsnotification-resource-type"></a>tipo de recurso commsNotification

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | Os valores possíveis são: `created`, `updated`, `deleted`.      |
| Resourceurl pela       | String  | URI do recurso que foi alterado.                      |

> **Observação:** `resourceData` está disponível como dados adicionais. É uma entidade ou uma coleção de entidades, dependendo do número de alterações empacotadas na notificação.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
