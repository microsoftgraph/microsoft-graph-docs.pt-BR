---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: df535b89d238f31185ff187b207671337d05fd75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939085"
---
# <a name="property-resource-type"></a>tipo de recurso Property

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo    | Descrição                                        |
|:--------------|:--------|:---------------------------------------------------|
| IsQuery   | Booliano | Especifica se a propriedade é consultável. Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Opcional.  |
| isretrievable | Booliano | Especifica se a propriedade é recuperável. As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa. As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa. Opcional. |
| IsSearchable  | Booliano | Especifica se a propriedade é pesquisável. Somente propriedades do tipo `String` ou `Collection(String)` podem ser pesquisáveis. As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa. Opcional. |
| name          | String  | O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos `:`seguintes `;`: `,`, `(`, `)`, `[`, `]`, `{`, `}` `%` `$` `+` `!` `*` `=`,,,,,,,, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`. Obrigatório.                |
| type          | String  | O tipo de dados da propriedade. Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`. Obrigatório. |

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
