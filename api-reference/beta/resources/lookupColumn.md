---
author: JeremyKelley
description: A lookupColumn em um recurso columnDefinition indica que os valores da coluna são buscados em outra origem do site.
ms.date: 09/11/2017
title: LookupColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d5ddc59f00b171d6ba7d125e8a626aa97ddcfff9
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176556"
---
# <a name="lookupcolumn-resource-type"></a>Tipo de recurso LookupColumn

Namespace: microsoft.graph

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

| Propriedade                  | Tipo    | Descrição                                                                                                                                                                                                                |
| :------------------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **allowMultipleValues**   | booliano | Indica se vários valores podem ser selecionados da origem.                                                                                                                                                         |
| **allowUnlimitedLength**  | booliano | Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.                                                                                                                      |
| **columnName**            | string  | O nome da coluna de origem de pesquisa.                                                                                                                                                                                      |
| **listId**                | string  | O identificador exclusivo da lista de origem de pesquisa.                                                                                                                                                                           |
| **primaryLookupColumnId** | string  | Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*. Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->
