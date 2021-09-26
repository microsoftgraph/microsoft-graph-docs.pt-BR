---
title: Tipo de recurso searchBucket
description: Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9323bac249216cc1355e3944f4437d738da89b1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764588"
---
# <a name="searchbucket-resource-type"></a>Tipo de recurso searchBucket

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|aggregationFilterToken|Cadeia de caracteres| Um token que contém o filtro codificado para agregar as combinações de pesquisa pelo valor **de chave** específico. Para usar o filtro, passe o token como parte da propriedade **aggregationFilter** em um **objeto searchRequest,** no formato **"{field}: \\ "{aggregationFilterToken} \\ ""**. Veja um [exemplo](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).|
|Count|Int32| O número aproximado de combinações de pesquisa que compartilham o mesmo valor especificado na **propriedade key.** Observe que esse número não é o número exato de combinações.|
|chave|String| O valor discreto do campo em que uma agregação foi calculada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
