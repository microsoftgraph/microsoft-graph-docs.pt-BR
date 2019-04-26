---
title: tipo de recurso plannerPlanContext
description: O recurso **plannerPlanContext** representa a relação de um plannerPlan com uma experiência de usuário fora do Planner. Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 68d9233d2645c2176ad364fbcbfac869976f0586
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344442"
---
# <a name="plannerplancontext-resource-type"></a>tipo de recurso plannerPlanContext

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerPlanContext** representa a relação de um [plannerPlan](plannerplan.md) com uma experiência de usuário fora do Planner. Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.
A experiência que a entrada **plannerPlanContext** reenviado pode ser identificada com base na propriedade **ownerAppId** :
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: a entrada de contexto pertence ao Microsoft Teams.
 - 00000003-0000-0ff1-ce00-000000000000: a entrada de contexto pertence ao SharePoint.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Association|String|Anulável. Um tipo de associação definido pelo aplicativo entre o [plannerPlan](plannerplan.md) e o aplicativo. O aplicativo pode usar essas informações para rastrear diferentes tipos de relações com o mesmo [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Somente leitura. A data e hora em que o **plannerPlanContext** foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|displayNameSegments|Coleção String|Os segmentos do nome da experiência externa. Segmentos representam uma estrutura hierárquica que permite que outros aplicativos exibam a relação.|
|ownerAppId|String|Somente leitura. ID do aplicativo que criou o **plannerPlanContext**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
