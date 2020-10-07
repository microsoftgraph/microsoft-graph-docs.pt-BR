---
title: tipo de recurso searchBucket
description: Fornece uma agregação específica na resposta, o valor de um Bucket específico.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373850"
---
# <a name="searchbucket-resource-type"></a>tipo de recurso searchBucket

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|key|String| O valor discreto do campo no qual uma agregação foi calculada.|
|Count|Int32| O número aproximado de correspondências de pesquisa que compartilham o mesmo valor especificado na propriedade **Key** . Observe que esse número não é o número exato de correspondências.|
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
