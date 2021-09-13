---
title: Tipo de recurso TableRow
description: Representa uma linha em uma tabela.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 113e81f4730f093962a5ec5e0a2a2f19aa6fc57e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134392"
---
# <a name="tablerow-resource-type"></a>Tipo de recurso TableRow

Namespace: microsoft.graph

Representa uma linha em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableRow](../api/tablerow-get.md) | [WorkbookTableRow](tablerow.md) |Leia as propriedades e os relacionamentos do objeto tableRow.|
|[Update](../api/tablerow-update.md) | [WorkbookTableRow](tablerow.md)  |Atualize o objeto TableRow. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Retorna o objeto de intervalo associado a toda a linha.|
|[Delete](../api/tablerow-delete.md)|Nenhum(a)|Exclui a linha da tabela.|
|[List](../api/tablerow-list.md) | Conjunto [WorkbookTableRow](tablerow.md) |Obtenha uma coleção de objetos tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow](tablerow.md)|Obtém uma linha com base em sua posição na coleção.|
|[Add](../api/tablerowcollection-add.md)|[WorkbookTableRow](tablerow.md)|Adiciona uma nova linha à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|index|int|Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

