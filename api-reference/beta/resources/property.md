---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9862170dfcca0960ebd319089da70cca93782875
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990260"
---
# <a name="property-resource-type"></a>tipo de recurso Property

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                        |
|:--------------|:------------------|:---------------------------------------------------|
| aliases       | Coleção de cadeias de caracteres | Um conjunto de aliases ou um nome amigável para a propriedade. Máximo de 32 caracteres. Cada cadeia de caracteres não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `;` `,` , `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` , `|` `` ` `` `^` ,,,,,,,,, Opcional.  |
| IsQuery   | Booliano           | Especifica se a propriedade é consultável. Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Opcional.  |
| isRefinable   | Booliano           | Especifica se a propriedade é refinável.  As propriedades refinável podem ser usadas para filtrar os resultados da pesquisa na [API de pesquisa](search-api-overview.md) e adicionar um controle de refinamento na experiência do usuário do Microsoft Search. Opcional.  |
| isretrievable | Booliano           | Especifica se a propriedade é recuperável. As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa. As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa. Opcional. |
| IsSearchable  | Booliano           | Especifica se a propriedade é pesquisável. Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis. As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa. Opcional. |
| Legendas        | Coleção de cadeias de caracteres | Especifica uma ou mais marcas conhecidas e adicionadas a uma propriedade. Os rótulos ajudam a pesquisa da Microsoft a entender a semântica dos dados na conexão. A adição de rótulos apropriados resultaria em uma experiência de pesquisa avançada (por exemplo, maior relevância). Rótulos com suporte:,,,,, `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` , `lastModifiedDateTime` , `fileName` e `fileExtension` . Opcional. |
| nome          | String            | O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` , `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` , Obrigatório.                |
| tipo          | String            | O tipo de dados da propriedade. Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`. Obrigatório. |

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
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
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
