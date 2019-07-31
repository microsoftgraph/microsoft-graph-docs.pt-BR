---
author: daspek
description: O recurso Entidadeitemactivitystat fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.
ms.date: 09/14/2017
title: Entidadeitemactivitystat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61c410d807869615ed35365743d1ae87b5b6e890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967088"
---
# <a name="itemactivitystat-resource-type"></a>tipo de recurso Entidadeitemactivitystat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.

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

| Propriedade         | Tipo                    | Descrição
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Indica que as estatísticas neste intervalo são baseadas em dados incompletos. Somente leitura.
| istendência       | Booliano                 | Indica se o item é "Trending". Somente leitura.
| startDateTime    | DateTimeOffset          | Quando o intervalo é iniciado. Somente leitura.
| endDateTime      | DateTimeOffset          | Quando o intervalo termina. Somente leitura.
| create           | [itemActionStat][]      | Estatísticas sobre as ações de **criação** neste intervalo. Somente leitura.
| edit             | [itemActionStat][]      | Estatísticas sobre as ações de **edição** neste intervalo. Somente leitura.
| delete           | [itemActionStat][]      | Estatísticas sobre as ações de **exclusão** neste intervalo. Somente leitura.
| move             | [itemActionStat][]      | Estatísticas sobre as ações de **movimentação** neste intervalo. Somente leitura.
| Access           | [itemActionStat][]      | Estatísticas sobre as ações de **acesso** neste intervalo. Somente leitura.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:---------------------------
| activities        | Conjunto [itemActivity][] | Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .

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
