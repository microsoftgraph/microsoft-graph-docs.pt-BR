---
author: daspek
ms.author: dspektor
title: tipo de recurso do multianalytics
description: O objeto PostItem fornece análises sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 879fad9ae77f065a7235a6adbfde5f742a1970f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009293"
---
# <a name="itemanalytics-resource-type"></a>tipo de recurso do multianalytics

Namespace: microsoft.graph

O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.

Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.

>**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                 | Descrição
|:--------------|:---------------------|:--------------------------------------
| Época       | [itemActivityStat][] | Análise sobre o ciclo de vida do item.
| lastSevenDays | [itemActivityStat][] | Análise dos últimos sete dias.

[itemActivityStat]: itemactivitystat.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md

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

