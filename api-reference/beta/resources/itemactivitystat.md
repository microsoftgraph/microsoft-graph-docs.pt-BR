---
author: daspek
description: O recurso Entidadeitemactivitystat fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.
ms.date: 09/14/2017
title: Entidadeitemactivitystat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c21183911e111b2070d463f4552f913d93780493
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075655"
---
# <a name="itemactivitystat-resource-type"></a>tipo de recurso Entidadeitemactivitystat

Namespace: microsoft.graph

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

## <a name="relationships"></a>Relacionamentos

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


