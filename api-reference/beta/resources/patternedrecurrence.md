---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: 9be505b1c9de704f1113e6cac3daa0396ca0949e
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545116"
---
# <a name="patternedrecurrence-resource-type"></a>Tipo de recurso patternedRecurrence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O padrão e o intervalo da recorrência. Esse objeto compartilhado é usado para definir a recorrência de avaliações de [acesso,](accessreviewscheduledefinition.md)eventos de calendário [e](event.md)atribuições de pacote de acesso [no](accesspackageassignment.md) Azure AD.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|pattern|[recurrencePattern](recurrencepattern.md)|A frequência de um evento. Não especifique para uma revisão de acesso único. <br/><br/> Para análises de acesso: <li>Não especifique essa propriedade para uma revisão de acesso único. <li>  Somente **as** propriedades interval , **dayOfMonth** e **type** ( , ) `weekly` de `absoluteMonthly` [recurrencePattern](recurrencepattern.md) são suportadas.|
|intervalo|[recurrenceRange](recurrencerange.md)|A duração de um evento.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


