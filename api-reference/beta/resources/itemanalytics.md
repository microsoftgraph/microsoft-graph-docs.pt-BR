---
author: daspek
description: O recurso do Microsoft Analytics oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.
ms.date: 09/14/2017
title: O naanalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967090"
---
# <a name="itemanalytics-resource-type"></a>tipo de recurso do multianalytics

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
| Época       | [itemActivityStat][] | Análise sobre o ciclo de vida do item.
| lastSevenDays | [itemActivityStat][] | Análise dos últimos sete dias.

[itemActivityStat]: itemactivitystat.md


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
