---
title: Tipo de recurso workbookTableColumn
description: Representa uma coluna em uma tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 27a44c0b75cfe62d27b1187616f9626772575cf4
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034008"
---
# <a name="workbooktablecolumn-resource-type"></a>Tipo de recurso workbookTableColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coluna em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableColumn](../api/tablecolumn-get.md) | [workbookTableColumn](workbooktablecolumn.md) |Leia as propriedades e os relacionamentos do objeto tableColumn.|
|[Update](../api/tablecolumn-update.md) | [workbookTableColumn](workbooktablecolumn.md) |Atualize o objeto TableColumn. |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado ao corpo de dados da coluna.|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da coluna.|
|[Range](../api/tablecolumn-range.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado a toda a coluna.|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado à linha de totais da coluna.|
|[Delete](../api/tablecolumn-delete.md)|Nenhum|Exclui a coluna da tabela.|
|[List](../api/tablecolumn-list.md) | [coleção workbookTableColumn](workbooktablecolumn.md) |Obtenha uma coleção de objetos tableColumn. |
|[Itemat](../api/tablecolumncollection-itemat.md)|[workbookTableColumn](workbooktablecolumn.md)|Obtém uma coluna com base em sua posição na coleção.|
|[Add](../api/tablecolumncollection-add.md)|[workbookTableColumn](workbooktablecolumn.md)|Adiciona uma nova coluna à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|Retorna uma chave exclusiva que identifica a coluna na tabela. Somente leitura.|
|índice|int|Retorna o número de índice da coluna na coleção de colunas da tabela. Indexado com zero. Somente leitura.|
|nome|string|Retorna o nome da coluna da tabela.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|filter|[workbookFilter](workbookfilter.md)|Recupera o filtro aplicado à coluna. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


