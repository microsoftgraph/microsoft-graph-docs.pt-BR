---
title: Tipo de recurso followupFlag
description: 'Permite configurar um sinalizador em um item para que o usuário acompanhe posteriormente. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e45fd04fa084fbc26c8eb43316de2f25b70cc0b7e2d5aa721bfc26ab1cfd0063
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180849"
---
# <a name="followupflag-resource-type"></a>Tipo de recurso followupFlag

Namespace: microsoft.graph


Permite configurar um sinalizador em um item para que o usuário acompanhe posteriormente.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Data e hora em que o acompanhamento foi concluído.|
|dueDateTime|**dateTimeTimeZone**|A data e a hora em que o acompanhamento deve ser concluído. **Observação**: Para definir a data de vencimento, você também deve especificar o `startDateTime` ; caso contrário, você receberá uma `400 Bad Request` resposta.|
|flagStatus|followupFlagStatus|O status de acompanhamento de um item. Os valores possíveis são: `notFlagged`, `complete` e `flagged`.|
|startDateTime|**dateTimeTimeZone**|Data e hora em que o acompanhamento deve começar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

