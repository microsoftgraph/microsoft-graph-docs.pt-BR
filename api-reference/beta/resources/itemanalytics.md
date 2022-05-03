---
author: daspek
description: O recurso itemAnalytics fornece análise sobre atividades que ocorreram em um item. No momento, esse recurso só está disponível SharePoint e OneDrive for Business.
ms.date: 09/14/2017
title: ItemAnalytics
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 15bd59f04384f2b18329f581f568ee465a86c040
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176929"
---
# <a name="itemanalytics-resource-type"></a>Tipo de recurso itemAnalytics

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso itemAnalytics** fornece análise sobre atividades que ocorreram em um item. No momento, esse recurso só está disponível SharePoint e OneDrive for Business.

Você também pode usar a API [getActivitiesByInterval][] para recuperar a análise em um intervalo ou intervalo de tempo personalizado.

>**Nota:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).

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
| lastSevenDays | [itemActivityStat][] | Análise dos últimos sete dias.

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

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


