---
title: tipo de recurso workbookTableRow
description: Representa uma linha em uma tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e20811129b069011db8b6a8ab9a6b762603b7600
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023748"
---
# <a name="workbooktablerow-resource-type"></a>tipo de recurso workbookTableRow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableRow](../api/tablerow-get.md) | [workbookTableRow](workbooktablerow.md) |Leia as propriedades e os relacionamentos do objeto tableRow.|
|[Update](../api/tablerow-update.md) | [workbookTableRow](workbooktablerow.md)  |Atualize o objeto TableRow. |
|[Range](../api/tablerow-range.md)|[workbookRange](workbookrange.md)|Retorna o objeto de intervalo associado a toda a linha.|
|[Delete](../api/tablerow-delete.md)|Nenhum|Exclui a linha da tabela.|
|[List](../api/tablerow-list.md) | coleção [workbookTableRow](workbooktablerow.md) |Obtenha uma coleção de objetos tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[workbookTableRow](workbooktablerow.md)|Obtém uma linha com base em sua posição na coleção.|
|[Add](../api/tablerowcollection-add.md)|[workbookTableRow](workbooktablerow.md)|Adiciona uma nova linha à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|index|int|Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


