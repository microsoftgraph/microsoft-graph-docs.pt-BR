---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: O naAnalytics
localization_priority: Normal
ms.openlocfilehash: 2869655b3b645fc8d30ceec3867c28ca81ac9d51
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345447"
---
# <a name="itemanalytics-resource-type"></a>tipo de recurso do multiAnalytics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.

Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.

>**Observação:** O **** recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                 | Descrição
|:--------------|:---------------------|:--------------------------------------
| Época       | [Entidadeitemactivitystat][] | Análise sobre o ciclo de vida do item.
| lastSevenDays | [Entidadeitemactivitystat][] | Análise dos últimos sete dias.

[Entidadeitemactivitystat]: itemactivitystat.md


[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->
