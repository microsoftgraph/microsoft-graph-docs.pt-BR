---
title: tipo de recurso de propriedade
description: Uma definição de propriedade de esquema para uma Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d15091c9a4f637019cf85cc55011feec86ce44f
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665750"
---
# <a name="property-resource-type"></a>tipo de recurso de propriedade

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma [definição de propriedade](externalconnectors-schema.md) de esquema para uma Pesquisa da Microsoft [conexão](externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                        |
|:--------------|:------------------|:---------------------------------------------------|
| aliases       | Coleção de cadeias de caracteres | Um conjunto de aliases ou nomes amigáveis para a propriedade. Máximo de 32 caracteres. Cada cadeia de caracteres não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` , , , , `*` , `=` `&` `?` `@` , `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` . Opcional.  |
| isQueryable   | booliano           | Especifica se a propriedade pode ser consultada. As propriedades queryable podem ser usadas em consultas [KQL (Keyword Query Language).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Opcional.  |
| isRefinable   | booliano           | Especifica se a propriedade é refinável.  As propriedades refináveis podem ser usadas para filtrar os resultados da pesquisa na [API](search-api-overview.md) de Pesquisa e adicionar um controle refinador na experiência Pesquisa da Microsoft usuário. Opcional.  |
| isRetrievable | booliano           | Especifica se a propriedade é recuperável. As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa. Propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa. Opcional. |
| isSearchable  | booliano           | Especifica se a propriedade é pesquisável. Somente propriedades do tipo `string` ou `stringCollection` podem ser pesquisáveis. Propriedades não pesquisáveis não são adicionadas ao índice de pesquisa. Opcional. |
| labels        | coleção microsoft.graph.externalConnectors.label | Especifica uma ou mais marcas conhecidas adicionadas a uma propriedade. Os rótulos Pesquisa da Microsoft entender a semântica dos dados na conexão. Adicionar rótulos apropriados resultaria em uma experiência de pesquisa aprimorada (por exemplo, melhor relevância). Opcional.<br><br>Os valores possíveis são: `title` , , , , , , , , , `url` , , `createdBy` , , , `lastModifiedBy` , `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `unknownFutureValue` `iconUrl` `containerName` `containerUrl` . Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include-unknown-enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `iconUrl` , , `containerName` `containerUrl` .|
| nome          | Cadeia de caracteres            | O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , , `;` `,` `(` `)` `[` `]` , `{` `}` , , `%` , , , `$` `+` `!` `*` `=` `&` `?` `@` `#` , `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` . Obrigatório.                |
| type          | microsoft.graph.externalConnectors.propertyType         | O tipo de dados da propriedade. Os valores possíveis são: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`. Obrigatório. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
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
