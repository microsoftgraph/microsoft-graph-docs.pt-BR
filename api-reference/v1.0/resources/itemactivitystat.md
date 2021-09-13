---
author: daspek
title: Tipo de recurso itemActivityStat
description: O objeto ItemActivityStat fornece informações sobre atividades que ocorreram em um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 97702f31f8b6125b06d3c34eba9eda596604422c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113662"
---
# <a name="itemactivitystat-resource-type"></a>Tipo de recurso itemActivityStat

Namespace: microsoft.graph

O **recurso itemActivityStat** fornece informações sobre atividades que ocorreram dentro de um intervalo de tempo.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                    | Descrição
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Indica que as estatísticas nesse intervalo se baseiam em dados incompletos. Somente leitura.
| isTrending       | Booliano                 | Indica se o item está "em tendência". Somente leitura.
| startDateTime    | DateTimeOffset          | Quando o intervalo é iniciado. Somente leitura.
| endDateTime      | DateTimeOffset          | Quando o intervalo terminar. Somente leitura.
| create           | [itemActionStat][]      | Estatísticas sobre as ações **de** criação nesse intervalo. Somente leitura.
| edit             | [itemActionStat][]      | Estatísticas sobre as ações **de edição** neste intervalo. Somente leitura.
| delete           | [itemActionStat][]      | Estatísticas sobre as ações **de exclusão** nesse intervalo. Somente leitura.
| move             | [itemActionStat][]      | Estatísticas sobre as ações **de movimentação** nesse intervalo. Somente leitura.
| access           | [itemActionStat][]      | Estatísticas sobre as ações **de acesso** nesse intervalo. Somente leitura.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:---------------------------
| activities        | Conjunto [itemActivity][] | Expõe o **itemActivities** representado neste **recurso itemActivityStat.**

[itemActivity]: itemactivity.md

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

