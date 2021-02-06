---
title: tipo de recurso filter
description: Determina quais objetos devem ser provisionados para o aplicativo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8c461dffab9af810d20f6b866134ecc5d4238eb1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133928"
---
# <a name="filter-resource-type"></a>tipo de recurso filter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, talvez você queira provisionar apenas usuários localizados nos EUA. Quando um filtro de scoping estiver presente, os objetos que não satisfazem o filtro serão ignorados durante a sincronização.

O filtro faz parte do [mapeamento de objetos.](synchronization-objectmapping.md) Ele consiste em vários conjuntos de grupos de filtros, e cada grupo de filtros contém uma ou mais cláusulas. Um objeto é considerado no escopo do grupo (o grupo é avaliado para ) somente se todas as cláusulas do grupo `true` são avaliadas para `true` .

Um objeto é considerado no escopo do conjunto de grupos (o conjunto de grupos é avaliado como ) se qualquer um dos grupos no conjunto `true` for avaliado como `true` .

Para obter mais informações, consulte [Provisionamento de aplicativo baseado em atributo com filtros de scoping](/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryFilterGroups|[coleção filterGroup](synchronization-filtergroup.md)|`*Experimental*` Conjunto de grupos de filtros usado para decidir se determinado objeto pertence e deve ser processado como parte desse mapeamento de objeto. Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*.|
|grupos|[coleção filterGroup](synchronization-filtergroup.md)|Conjunto de grupos de filtros usado para decidir se determinado objeto está no escopo do provisionamento. **Este é o filtro que deve ser usado na maioria dos casos.** Se um objeto usado para satisfazer esse filtro em um dado momento e, em seguida, o objeto ou o filtro foi alterado para que o filtro não seja mais satisfeito, esse objeto *será des-provisionado". Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*.|
|inputFilterGroups|[coleção filterGroup](synchronization-filtergroup.md)|`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory. Se um objeto não satisfaça esse filtro, ele não será processado ainda mais. É importante entender que, se um objeto usado para satisfazer esse filtro em um determinado momento e, em seguida, o objeto ou o filtro foi alterado para que o filtro não seja mais satisfeito, esse objeto NÃO será *des* provisionado. Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


