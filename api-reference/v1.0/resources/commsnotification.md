---
title: Tipo de recurso commsNotification
description: Tipo de base de notificação de comunicações publicado pelos servidores de Comunicações para notificar as alterações.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff7d46a6d081889897940a93d5d111ffa2956a21fc61411060cad08ed2f7d5ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252015"
---
# <a name="commsnotification-resource-type"></a>Tipo de recurso commsNotification

Namespace: microsoft.graph

Tipo de base de notificação de comunicações publicado pelos servidores de Comunicações para notificar as alterações.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    | Descrição                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | Os valores possíveis são: `created`, `updated`, `deleted`.      |
| resourceUrl       | Cadeia de caracteres  | URI do recurso que foi alterado.                      |

> **Observação:** `resourceData` está disponível como dados adicionais. É uma entidade ou uma coleção de entidades, dependendo do número de alterações empacotada na notificação.

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

