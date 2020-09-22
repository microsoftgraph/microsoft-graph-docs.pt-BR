---
title: tipo de recurso searchBucket
description: Fornece uma agregação específica na resposta, o valor de um Bucket específico.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193822"
---
# <a name="searchbucket-resource-type"></a>tipo de recurso searchBucket

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega. 



## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|key|String| O valor discreto do campo no qual uma agregação foi calculada.|
|Count|Int32| O número de correspondências de pesquisa que compartilham o mesmo valor especificado na propriedade **Key** . |
|aggregationFilterToken|String| Um token contendo o filtro codificado para agregar correspondências de pesquisa pelo valor da **chave** específica. Para usar o filtro, passe o token como parte da propriedade **aggregationFilter** em um objeto **searchRequest** , no formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**. Veja um [exemplo](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).|

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
