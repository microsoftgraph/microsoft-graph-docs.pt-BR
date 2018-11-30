---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033465"
---
# <a name="itemactivitystat-resource-type"></a>tipo de recurso de itemActivityStat

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **itemActivityStat** fornece informações sobre atividades realizadas dentro de um intervalo de tempo.

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
| incompleteData   | [incompleteData][]      | Indica que as estatísticas nesse intervalo são baseadas em dados incompletos. Somente leitura.
| isTrending       | Booliano                 | Indica se o item é "tendências". Somente leitura.
| startDateTime    | DateTimeOffset          | Quando o intervalo for iniciado. Somente leitura.
| endDateTime      | DateTimeOffset          | Quando o intervalo termina. Somente leitura.
| create           | [itemActionStat][]      | Estatísticas sobre as ações **criar** nesse intervalo. Somente leitura.
| edit             | [itemActionStat][]      | Estatísticas sobre as ações de **Editar** nesse intervalo. Somente leitura.
| delete           | [itemActionStat][]      | Estatísticas sobre as ações **Excluir** nesse intervalo. Somente leitura.
| move             | [itemActionStat][]      | Estatísticas sobre as ações de **Mover** nesse intervalo. Somente leitura.
| acesso           | [itemActionStat][]      | Estatísticas sobre as ações de **acesso** nesse intervalo. Somente leitura.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:---------------------------
| activities        | Conjunto [itemActivity][] | Expõe **itemActivities** representados neste recurso **itemActivityStat** .

[itemActivity]: itemactivity.md

## <a name="remarks"></a>Comentários

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
