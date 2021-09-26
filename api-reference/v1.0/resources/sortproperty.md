---
title: Tipo de recurso sortProperty
description: Indica a ordem para classificar os resultados da pesquisa
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 822819ba68ba6786da111d8976c76fdcd30e591d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514323"
---
# <a name="sortproperty-resource-type"></a>Tipo de recurso sortProperty

Namespace: microsoft.graph

Indica a ordem para classificar os resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|name|Cadeia de caracteres|O nome da propriedade a ser classificação. Obrigatório.|
|isDescending|Boolean|`True` se a ordem de classificação estiver decrescente. O padrão `false` é , com a ordem de classificação como crescente. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortProperty",
  "baseType": null
}-->

```json
{
  "name": "String",
  "isDescending": "true"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->