---
title: tipo de recurso workbookTableRow
description: Representa uma linha em uma tabela.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4b546e3593668c167479d18bcc06e1d61f59fbb4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777147"
---
# <a name="workbooktablerow-resource-type"></a>tipo de recurso workbookTableRow

Namespace: microsoft.graph

Representa uma linha em uma tabela.


## <a name="methods"></a>Métodos

### <a name="manage-workbooktablerow"></a>Gerenciar workbookTableRow
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookTableRow](../api/tablerow-get.md) | [WorkbookTableRow]( workbooktablerow.md) |Leia as propriedades e os relacionamentos do objeto tableRow.|
|[Update](../api/tablerow-update.md) | [WorkbookTableRow]( workbooktablerow.md) |Atualizar o objeto workbookTableRow. |
|[Delete](../api/tablerow-delete.md)|Nenhum|Exclui a linha da tabela.|
|[Criar workbookTableRow](../api/table-post-rows.md)|[WorkbookTableRow]( workbooktablerow.md)|Adiciona linhas à tabela.|
|[Range](../api/tablerow-range.md)|[Range](range.md)|Retorna o objeto de intervalo associado a toda a linha.|
|[List](../api/tablerow-list.md) | [workbookTableRow]( workbooktablerow.md) collection |Obtenha uma coleção de objetos tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow]( workbooktablerow.md)|Obtém uma linha com base em sua posição na coleção.|
|[Add](../api/tablerowcollection-add.md)|[WorkbookTableRow]( workbooktablerow.md)|Adiciona uma nova linha à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|índice|Int32|Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.|
|values|[Json](../resources/json.md)|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "index": "Integer",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookTableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

