---
title: Tipo de recurso workbookTableColumn
description: Representa uma coluna em uma tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 85a8c4b53eb39ae440946872718447f272ef841b
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033908"
---
# <a name="workbooktablecolumn-resource-type"></a>Tipo de recurso workbookTableColumn

Namespace: microsoft.graph

Representa uma coluna em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableColumn](../api/tablecolumn-get.md) | [WorkbookTableColumn](workbooktablecolumn.md) |Leia as propriedades e os relacionamentos do objeto tableColumn.|
|[Update](../api/tablecolumn-update.md) | [WorkbookTableColumn](workbooktablecolumn.md) |Atualize o objeto TableColumn. |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado ao corpo de dados da coluna.|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.|
|[Range](../api/tablecolumn-range.md)|[Range](range.md)|Obtém o objeto de intervalo associado a toda a coluna.|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de totais da coluna.|
|[Delete](../api/tablecolumn-delete.md)|Nenhum(a)|Exclui a coluna da tabela.|
|[List](../api/tablecolumn-list.md) | Conjunto [WorkbookTableColumn](workbooktablecolumn.md) |Obtenha uma coleção de objetos tableColumn. |
|[Itemat](../api/tablecolumncollection-itemat.md)|[WorkbookTableColumn](workbooktablecolumn.md)|Obtém uma coluna com base em sua posição na coleção.|
|[Add](../api/tablecolumncollection-add.md)|[WorkbookTableColumn](workbooktablecolumn.md)|Adiciona uma nova coluna à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|Retorna uma chave exclusiva que identifica a coluna na tabela. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.|
|index|int|Retorna o número de índice da coluna na coleção de colunas da tabela. Indexado com zero. Somente leitura.|
|nome|string|Retorna o nome da coluna da tabela.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|filter|[WorkbookFilter](filter.md)|Recupera o filtro aplicado à coluna. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": "1024",
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

