---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842410"
---
# <a name="itemanalytics-resource-type"></a>tipo de recurso de itemAnalytics

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
