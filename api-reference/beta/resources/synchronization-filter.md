---
title: tipo de recurso de filtro
description: Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA. Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894408"
---
# <a name="filter-resource-type"></a>tipo de recurso de filtro

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA. Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.

Filtro faz parte do [mapeamento do objeto](synchronization-objectmapping.md). Ele consiste em vários conjuntos de grupos de filtro, e cada grupo de filtro contém uma ou mais cláusulas. Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.

Um objeto é considerado no escopo para conjunto de grupos (conjunto de grupo é avaliado para `true`) se qualquer um dos grupos no conjunto é avaliada para `true`.

Para obter mais informações, consulte [aplicativo baseado no atributo provisionamento com filtros de escopo](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryFilterGroups|coleção [filterGroup](synchronization-filtergroup.md)|`*Experimental*`Filtro de conjunto de grupo usado para decidir se determinados objeto pertence e devem ser processadas como parte desse mapeamento do objeto. Um objeto é considerado no escopo *se qualquer um dos grupos na coleção é avaliada para `true` *.|
|grupos|coleção [filterGroup](synchronization-filtergroup.md)|Filtro usado para decidir se determinados objeto está no escopo de provisionamento do conjunto de grupos. **Este é o filtro que deve ser usado na maioria dos casos**. Se um objeto usado para atender a esse filtro em um determinado momento e, em seguida, o objeto ou o filtro foi alterado por esse filtro não é mais, satisfeito tal objeto * irá obter provisionado desprovisionamento ". Um objeto é considerado no escopo *se qualquer um dos grupos na coleção é avaliada para `true` *.|
|inputFilterGroups|coleção [filterGroup](synchronization-filtergroup.md)|`*Experimental*`Filtro de conjunto de grupo usado para filtrar os objetos no estágio inicial de leitura-los do diretório. Se um objeto não satisfizerem esse filtro não será mais processado. É importante entender é que se um objeto usado para atender a esse filtro em um determinado momento, e, em seguida, o objeto ou o filtro foi alterado isso esse filtro não está mais satisfeito, tais objeto *não sejam provisionados desprovisionamento*. Um objeto é considerado no escopo *se qualquer um dos grupos na coleção é avaliada para `true` *. |

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
