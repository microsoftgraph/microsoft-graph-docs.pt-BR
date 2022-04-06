---
author: daspek
description: O recurso itemActivityStat fornece informações sobre atividades que ocorreram dentro de um intervalo de tempo.
ms.date: 09/14/2017
title: ItemActivityStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 27089dcb5e9223710edb60bbdafe88fa0b3f8099
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723902"
---
# <a name="itemactivitystat-resource-type"></a>Tipo de recurso itemActivityStat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso itemActivityStat** fornece informações sobre atividades que ocorreram dentro de um intervalo de tempo.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo               | Descrição                                                                             |
| :------------- | :----------------- | :-------------------------------------------------------------------------------------- |
| incompleteData | [incompleteData][] | Indica que as estatísticas nesse intervalo se baseiam em dados incompletos. Somente leitura. |
| isTrending     | Booliano            | Indica se o item está "em tendência". Somente leitura.                                    |
| startDateTime  | DateTimeOffset     | Quando o intervalo é iniciado. Somente leitura.                                                    |
| endDateTime    | DateTimeOffset     | Quando o intervalo terminar. Somente leitura.                                                      |
| create         | [itemActionStat][] | Estatísticas sobre as ações **de** criação nesse intervalo. Somente leitura.                    |
| edit           | [itemActionStat][] | Estatísticas sobre as ações **de edição** neste intervalo. Somente leitura.                      |
| delete         | [itemActionStat][] | Estatísticas sobre as ações **de exclusão** nesse intervalo. Somente leitura.                    |
| move           | [itemActionStat][] | Estatísticas sobre as ações **de movimentação** nesse intervalo. Somente leitura.                      |
| access         | [itemActionStat][] | Estatísticas sobre as ações **de acesso** nesse intervalo. Somente leitura.                    |

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Relações

| Relação | Tipo                        | Descrição                                                                       |
| :----------- | :-------------------------- | :-------------------------------------------------------------------------------- |
| activities   | Conjunto [itemActivity][] | Expõe o **itemActivities** representado neste **recurso itemActivityStat** . |

[itemActivity]: itemactivity.md

## <a name="remarks"></a>Comentários

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
