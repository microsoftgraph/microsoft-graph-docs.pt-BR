---
author: daspek
title: Tipo de recurso itemAnalytics
description: O objeto ItemAnalytics fornece análises sobre atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96ad65ef5cc8907663a9ca67e5ea2b7546b8fa03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238656"
---
# <a name="itemanalytics-resource-type"></a>Tipo de recurso itemAnalytics

Namespace: microsoft.graph

O **recurso itemAnalytics** fornece análises sobre atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.

Você também pode usar a API [getActivitiesByInterval][] para recuperar a análise em um intervalo de tempo ou intervalo personalizado.

>**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                 | Descrição
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Análise sobre o tempo de vida do item.
| lastSevenDays | [itemActivityStat][] | Análise dos últimos sete dias.

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

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

