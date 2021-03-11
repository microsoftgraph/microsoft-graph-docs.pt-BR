---
title: Tipo de recurso plannerRecentPlanReference
description: 'O **tipo de recurso plannerRecentPlanReference** repesenta uma referência a um plannerPlan que foi exibido recentemente por um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8a8fbf3ce9f39c49dde4bbeee96a3aab15a00077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720974"
---
# <a name="plannerrecentplanreference-resource-type"></a>Tipo de recurso plannerRecentPlanReference

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **tipo de recurso plannerRecentPlanReference** repesenta uma referência a um [plannerPlan](plannerplan.md) que foi exibido recentemente por um usuário. O **plannerRecentPlanReferences** para um usuário é explicitamente mantido por aplicativos. Qualquer aplicativo que implemente o recurso de planos recentes deve registrar quando o usuário exibiu pela última vez um plano e atualizar as entradas **do plannerRecentPlanReference** de acordo.
Os aplicativos devem observar que as entradas **plannerRecentPlanReference** podem fazer referência a **plannerPlans excluídos,** que o usuário não pode mais acessar ou que foram atualizados com um título diferente.
Recomendamos que os aplicativos notifiquem os usuários quando houver discrepâncias e mantenham as entradas atualizadas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|A data e a hora em que o plano foi exibido pela última vez pelo usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|planTitle|Cadeia de caracteres|O título do plano no momento em que o usuário o exibiu.|

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


