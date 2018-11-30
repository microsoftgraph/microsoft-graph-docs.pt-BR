---
title: tipo de recurso de plannerRecentPlanReference
description: 'O recurso de **plannerRecentPlanReference** digite representa uma referência a um plannerPlan que recentemente foi exibido por um usuário. '
ms.openlocfilehash: ac774ffbf7ebdfe45211cf50c2ce065921de30f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033862"
---
# <a name="plannerrecentplanreference-resource-type"></a>tipo de recurso de plannerRecentPlanReference

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **plannerRecentPlanReference** digite representa uma referência a um [plannerPlan](plannerplan.md) recentemente foi exibido por um usuário. O **plannerRecentPlanReferences** para um usuário explicitamente são mantidas por aplicativos. Qualquer aplicativo que implementa o recurso de planos recente deve gravar quando o usuário visualizado por último entradas de **plannerRecentPlanReference** de atualização e um plano de acordo.
Aplicativos Lembre-se de que as entradas de **plannerRecentPlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode acessar ou que foram atualizados com um título diferente.
É recomendável que os aplicativos notificar os usuários quando houver discrepâncias e manter as entradas atualizado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|A data e hora que o plano foi visualizado por último pelo usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|planTitle|String|O título do plano no momento em que o usuário exibidos-lo.|

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
