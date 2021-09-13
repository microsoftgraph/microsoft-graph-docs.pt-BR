---
title: Tipo de recurso followupFlag
description: 'Permite configurar um sinalizador em um item para que o usuário acompanhe posteriormente. '
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 17d9b1d2e12a33d5df53acf434489377089d89ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078851"
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

