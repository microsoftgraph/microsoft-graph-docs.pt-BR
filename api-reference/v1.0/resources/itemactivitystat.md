---
author: daspek
title: Tipo de recurso itemActivityStat
description: O objeto ItemActivityStat fornece informações sobre atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 8fe252948bc717584204ec9be0c34cd23e5799d1bf382ef9aa45b28cfc21d6ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130083"
---
# <a name="itemactivitystat-resource-type"></a>Tipo de recurso itemActivityStat

Namespace: microsoft.graph

O **recurso itemActivityStat** fornece informações sobre atividades que ocorreram dentro de um intervalo de tempo.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                    | Descrição
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Indica que as estatísticas nesse intervalo se baseiam em dados incompletos. Apenas leitura.
| isTrending       | Booliano                 | Indica se o item está "em tendência". Apenas leitura.
| startDateTime    | DateTimeOffset          | Quando o intervalo é iniciado. Somente leitura.
| endDateTime      | DateTimeOffset          | Quando o intervalo terminar. Somente leitura.
| create           | [itemActionStat][]      | Estatísticas sobre as ações **de** criação nesse intervalo. Apenas leitura.
| edit             | [itemActionStat][]      | Estatísticas sobre as ações **de edição** neste intervalo. Apenas leitura.
| delete           | [itemActionStat][]      | Estatísticas sobre as ações **de exclusão** nesse intervalo. Somente leitura.
| move             | [itemActionStat][]      | Estatísticas sobre as ações **de movimentação** nesse intervalo. Apenas leitura.
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

