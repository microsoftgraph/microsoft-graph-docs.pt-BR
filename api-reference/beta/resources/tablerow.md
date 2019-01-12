---
title: Tipo de recurso TableRow
description: Representa uma linha em uma tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d96ef5c23361cd8b15b47af54a0584e21c48b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971657"
---
# <a name="tablerow-resource-type"></a>Tipo de recurso TableRow

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma linha em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableRow](../api/tablerow-get.md) | [TableRow](tablerow.md) |Leia as propriedades e os relacionamentos do objeto tableRow.|
|[Update](../api/tablerow-update.md) | [TableRow](tablerow.md)  |Atualize o objeto TableRow. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Retorna o objeto de intervalo associado a toda a linha.|
|[Delete](../api/tablerow-delete.md)|Nenhum|Exclui a linha da tabela.|
|[List](../api/tablerow-list.md) | Coleção [TableRow](tablerow.md) |Obtenha uma coleção de objetos tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|Obtém uma linha com base em sua posição na coleção.|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|Adiciona uma nova linha à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|índice|int|Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.|
|values|json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
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
