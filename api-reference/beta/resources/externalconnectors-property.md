---
title: tipo de recurso de propriedade
description: Uma definição de propriedade de esquema para uma Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68dfe94d81f4ae5347322ba17c02eb3dab5c15d7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467599"
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
| labels        | Coleção de cadeias de caracteres | Especifica uma ou mais marcas conhecidas adicionadas a uma propriedade. Os rótulos Pesquisa da Microsoft entender a semântica dos dados na conexão. Adicionar rótulos apropriados resultaria em uma experiência de pesquisa aprimorada (por exemplo, melhor relevância). Rótulos com `title` suporte: `url` , , , , , , , , `createdBy` , , , , , `lastModifiedBy` e `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `iconUrl` `containerName` `containerUrl` . Opcional. |
| nome          | String            | O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , , `;` `,` `(` `)` `[` `]` , `{` `}` , , `%` , , , `$` `+` `!` `*` `=` `&` `?` `@` `#` , `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` . Obrigatório.                |
| tipo          | String            | O tipo de dados da propriedade. Os valores possíveis são: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`. Obrigatório. |

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
