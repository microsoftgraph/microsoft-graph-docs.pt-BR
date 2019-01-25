---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514961"
---
# <a name="itemanalytics-resource-type"></a>tipo de recurso de itemAnalytics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de **itemAnalytics** fornece análise sobre atividades realizadas em um item. Este recurso só está disponível no SharePoint e o OneDrive for Business no momento.

Você também pode usar [getActivitiesByInterval][] API para recuperar o analytics sobre um intervalo de tempo personalizado ou um intervalo.

>**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).

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
| allTime       | [itemActivityStat][] | Análise sobre o tempo de vida do item.
| lastSevenDays | [itemActivityStat][] | Análise nos últimos sete dias.

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
