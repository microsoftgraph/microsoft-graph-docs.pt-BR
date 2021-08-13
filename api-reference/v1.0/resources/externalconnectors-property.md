---
title: tipo de recurso de propriedade
description: Uma definição de propriedade de esquema para uma Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fa8d162920c0a3678535ac6e8857191354216783b18ea348436b3d9681e1157f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229278"
---
# <a name="property-resource-type"></a>tipo de recurso de propriedade

Namespace: microsoft.graph.externalConnectors



Uma [definição de propriedade](externalconnectors-schema.md) de esquema para uma Pesquisa da Microsoft [conexão](externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aliases|String collection|Um conjunto de aliases ou nomes amigáveis para a propriedade. Máximo de 32 caracteres. Cada cadeia de caracteres não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` , , , , `*` , `=` `&` `?` `@` , `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` . Opcional.|
|isQueryable|Booliano|Especifica se a propriedade pode ser consultada. As propriedades queryable podem ser usadas em consultas [KQL (Keyword Query Language).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Opcional.|
|isRefinable|Booliano|Especifica se a propriedade é refinável.  As propriedades refináveis podem ser usadas para filtrar os resultados da pesquisa na [API](search-api-overview.md) de Pesquisa e adicionar um controle refinador na experiência Pesquisa da Microsoft usuário. Opcional.|
|isRetrievable|Booliano|Especifica se a propriedade é recuperável. As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa. Propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa. Opcional.|
|isSearchable|Booliano|Especifica se a propriedade é pesquisável. Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis. Propriedades não pesquisáveis não são adicionadas ao índice de pesquisa. Opcional.|
|labels|coleção microsoft.graph.externalConnectors.label|Especifica uma ou mais marcas conhecidas adicionadas a uma propriedade. Os rótulos Pesquisa da Microsoft entender a semântica dos dados na conexão. Adicionar rótulos apropriados resultaria em uma experiência de pesquisa aprimorada (por exemplo, melhor relevância). Os valores possíveis são `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName`, `fileExtension`, `unknownFutureValue`. Opcional.|
|nome|Cadeia de caracteres|O nome da propriedade. Máximo de 32 caracteres. Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , , `;` `,` `(` `)` `[` `]` , `{` `}` , , `%` , , , `$` `+` `!` `*` `=` `&` `?` `@` `#` , `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` . Obrigatório.|
|type|microsoft.graph.externalConnectors.propertyType|O tipo de dados da propriedade. Os valores possíveis são: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.property"
}
-->
``` json
{
  "name": "String",
  "type": "String",
  "isSearchable": "Boolean",
  "isRetrievable": "Boolean",
  "isQueryable": "Boolean",
  "isRefinable": "Boolean",
  "aliases": [
    "String"
  ],
  "labels": [
    "String"
  ]
}
```

