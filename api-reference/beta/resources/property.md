---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48a61c9f26a7f5b90e41fc2cd36334d4061449dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521380"
---
# <a name="property-resource-type"></a>tipo de recurso Property

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo    | Descrição                                        |
|:--------------|:--------|:---------------------------------------------------|
| IsQuery   | Boolean | Especifica se a propriedade é consultável. Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Opcional.  |
| isretrievable | Boolean | Especifica se a propriedade é recuperável. As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa. As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa. Opcional. |
| IsSearchable  | Boolean | Especifica se a propriedade é pesquisável. Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis. As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa. Opcional. |
| nome          | String  | O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos `:`seguintes `;`: `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?`,,,,,,,,,,,,, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`,,,,,,,,,,,,,,, Obrigatório.                |
| type          | String  | O tipo de dados da propriedade. Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`. Obrigatório. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
