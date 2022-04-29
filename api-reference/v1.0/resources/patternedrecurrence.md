---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23a0e22fe44cac84f017446326beea052e3c067c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133794"
---
# <a name="patternedrecurrence-resource-type"></a>Tipo de recurso patternedRecurrence

Namespace: microsoft.graph

O padrão e o intervalo da recorrência. Esse objeto compartilhado é usado para definir a recorrência dos seguintes objetos:
+ [objetos accessReviewScheduleDefinition](accessreviewscheduledefinition.md) Azure AD APIs de revisões de acesso
+ [objetos](event.md) de evento na API do calendário
+ [objetos unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) [e unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) no PIM
+ [objetos accessPackageAssignment](accesspackageassignment.md) Azure AD gerenciamento de direitos.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|pattern|[Recurrencepattern](recurrencepattern.md)|A frequência de um evento. <br/><br/> Para revisões de acesso: <li>Não especifique essa propriedade para uma revisão de acesso única. <li> Somente **as** **propriedades interval, dayOfMonth** e **type** (`weekly`, `absoluteMonthly`) de [recurrencePattern](recurrencepattern.md) têm suporte.|
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
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

