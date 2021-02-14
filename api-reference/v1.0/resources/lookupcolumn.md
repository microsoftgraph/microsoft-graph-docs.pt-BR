---
author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: A lookupColumn em um recurso columnDefinition indica que os valores da coluna são buscados em outra origem do site.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ec7da70a6f79793dbf12dbfea6c9fbfef53aaea9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239342"
---
# <a name="lookupcolumn-resource-type"></a>Tipo de recurso LookupColumn

Namespace: microsoft.graph

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

