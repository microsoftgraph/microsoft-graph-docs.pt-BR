---
title: tipo de recurso plannerRecentPlanReference
description: 'O tipo de recurso **plannerRecentPlanReference** representa uma referência a um plannerPlan que foi recentemente exibido por um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8439502aa1214e1ef2bbedd9864ef4724abf8021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965863"
---
# <a name="plannerrecentplanreference-resource-type"></a>tipo de recurso plannerRecentPlanReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **plannerRecentPlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi recentemente exibido por um usuário. O **plannerRecentPlanReferences** de um usuário é explicitamente mantido por aplicativos. Qualquer aplicativo que implemente o recurso de planos recentes deve registrar quando o usuário tiver exibido o último plano e atualizar as entradas de **plannerRecentPlanReference** de acordo.
Os aplicativos devem observar que as entradas do **plannerRecentPlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.
Recomendamos que os aplicativos Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|A data e a hora em que o plano foi exibido pela última vez pelo usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|planTitle|String|O título do plano no momento em que o usuário o exibiu.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
