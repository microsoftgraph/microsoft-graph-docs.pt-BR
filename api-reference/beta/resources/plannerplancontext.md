---
title: Tipo de recurso plannerPlanContext
description: O **recurso plannerPlanContext** representa a relação de um plannerPlan para uma experiência de usuário fora do Planner. Os planos no Planner podem aparecer em outras experiências, como o Microsoft Teams, para acompanhar o trabalho no contexto dessa experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720981"
---
# <a name="plannerplancontext-resource-type"></a>Tipo de recurso plannerPlanContext

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso plannerPlanContext** representa a relação de um [plannerPlan](plannerplan.md) para uma experiência de usuário fora do Planner. Os planos no Planner podem aparecer em outras experiências, como o Microsoft Teams, para acompanhar o trabalho no contexto dessa experiência. Experiências com links externos no [plannerPlanContextDetails](plannerplancontextdetails.md) podem ser exibidas em uma interface do usuário, permitindo que os usuários visite essas experiências.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|associationType|Cadeia de caracteres|Anulável. Um tipo de associação definido pelo aplicativo entre o [plannerPlan](plannerplan.md) e o aplicativo. O aplicativo pode usar essas informações para rastrear diferentes tipos de relações com o mesmo [plannerPlan](plannerplan.md).|
|createdDateTime|DateTimeOffset|Somente leitura. A data e a hora em que **o plannerPlanContext** foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|displayNameSegments|Coleção de cadeias de caracteres|Os segmentos do nome da experiência externa. Os segmentos representam uma estrutura hierárquica que permite que outros aplicativos exibem a relação.|
|isCreationContext|Booliano|Somente leitura. Indica se o plano é criado a partir do contexto especificado. Gerado automaticamente com base em se o contexto é especificado como parte da criação do plano.|
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
  "isCreationContext": false,
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


