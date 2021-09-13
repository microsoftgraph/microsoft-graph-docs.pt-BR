---
author: daspek
title: Tipo de recurso itemAnalytics
description: O objeto ItemAnalytics fornece análises sobre atividades que ocorreram em um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a9f1e6a70829d809feb6784441744ed74f8ea0d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084339"
---
# <a name="itemanalytics-resource-type"></a>Tipo de recurso itemAnalytics

Namespace: microsoft.graph

O **recurso itemAnalytics** fornece análises sobre atividades que ocorreram em um item. Atualmente, esse recurso só está disponível em SharePoint e OneDrive for Business.

Você também pode usar a API [getActivitiesByInterval][] para recuperar a análise em um intervalo ou intervalo de tempo personalizado.

>**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                 | Descrição
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Análise sobre o tempo de vida útil do item.
| lastSevenDays | [itemActivityStat][] | Análise dos últimos sete dias.

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka&quot;: &quot;oneDrive.analytics"
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

