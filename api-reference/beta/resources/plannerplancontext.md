---
title: tipo de recurso de plannerPlanContext
description: O recurso de **plannerPlanContext** representa a relação entre um plannerPlan a uma experiência de usuário fora do planejador. Planos no planejador podem ser exibidos em outras experiências, como Teams da Microsoft, para controlar o trabalho no contexto dessa experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509235"
---
# <a name="plannerplancontext-resource-type"></a>tipo de recurso de plannerPlanContext

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de **plannerPlanContext** representa a relação entre um [plannerPlan](plannerplan.md) a uma experiência de usuário fora do planejador. Planos no planejador podem ser exibidos em outras experiências, como Teams da Microsoft, para controlar o trabalho no contexto dessa experiência.
A experiência que a entrada **plannerPlanContext** reresents pode ser identificada com base na propriedade **ownerAppId** :
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: A entrada do contexto pertence à Microsoft Teams.
 - 00000003-0000-0ff1-CE00-000000000000: pertence a entrada do contexto do SharePoint.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|associationType|String|Anulável. Um tipo definido pelo aplicativo de associação entre o [plannerPlan](plannerplan.md) e o aplicativo. O aplicativo pode usar essas informações para rastrear diferentes tipos de relacionamentos para o mesmo [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Somente leitura. A data e hora em que o **plannerPlanContext** foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|displayNameSegments|String collection|Os segmentos do nome da experiência do externo. Segmentos representam uma estrutura hierárquica que permite a outros aplicativos exibir o relacionamento.|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
