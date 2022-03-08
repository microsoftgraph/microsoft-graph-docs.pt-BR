---
title: Tipo de recurso searchAnswer
description: A resposta de pesquisa é um tipo base para outras respostas de pesquisa.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 06fa9cfe754af55d4ee19640a9d75c00b7dbca2f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338116"
---
# <a name="searchanswer-resource-type"></a>Tipo de recurso searchAnswer

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A resposta de pesquisa é um tipo base para outras respostas de pesquisa, como recursos de [acrônimo](../resources/search-acronym.md), [indicador](../resources/search-bookmark.md) e [QnA](../resources/search-qna.md) . Inclui propriedades que se aplicam a outras entidades de resposta de pesquisa.


Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo (GUID) da resposta de pesquisa. Herdado da [entidade](../resources/entity.md).|
|displayName|Cadeia de caracteres|Nome da resposta de pesquisa exibido nos resultados da pesquisa.|
|descrição|String|Descrição da resposta de pesquisa mostrada na página de resultados da pesquisa.|
|webUrl|String|Link de URL de resposta de pesquisa. Quando os usuários clicarem nessa resposta de pesquisa nos resultados da pesquisa, eles irão para essa URL.|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Detalhes do usuário que criou ou modificou a resposta de pesquisa pela última vez. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Timestamp de quando a resposta de pesquisa é criada ou editada. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.searchAnswer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.searchAnswer",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

