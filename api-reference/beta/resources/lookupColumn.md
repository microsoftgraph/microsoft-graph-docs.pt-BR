---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1a38cc3e08917b0d4aa2a8df4943ebc932c937d4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480793"
---
# <a name="lookupcolumn-resource-type"></a>Tipo de recurso LookupColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **lookupColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são buscados em outra origem do site.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **lookupColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade             | Tipo    | Descrição
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | booliano | Indica se vários valores podem ser selecionados da origem.
| **allowUnlimitedLength**  | booliano | Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.
| **columnName**            | string  | O nome da coluna de origem de pesquisa.
| **listId**                | string  | O identificador exclusivo da lista de origem de pesquisa.
| **primaryLookupColumnId** | string  | Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*. Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
