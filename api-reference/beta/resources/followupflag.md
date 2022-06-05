---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: abheek-das
ms.openlocfilehash: 4f0ea743317aee80dd8f6bd1897069bbeb4e0fd7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899523"
---
# <a name="followupflag-resource-type"></a>Tipo de recurso followupFlag

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem [message](message.md) e [contact](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Data e hora em que o acompanhamento foi concluído.|
|dueDateTime|**dateTimeTimeZone**|A data e a hora em que o acompanhamento deve ser concluído. **Observação**: para definir a data de conclusão, você também deve especificar o `startDateTime`; caso contrário, você receberá uma `400 Bad Request` resposta.|
|flagStatus|Cadeia de caracteres|O status de acompanhamento de um item. Os valores possíveis são: `notFlagged`, `complete` e `flagged`.|
|startDateTime|**dateTimeTimeZone**|Data e hora em que o acompanhamento deve começar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


