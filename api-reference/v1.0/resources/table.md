---
title: Tipo de recurso Table
description: Representa uma tabela do Excel.
ms.openlocfilehash: 029f2477570b6ad1c85f6c92d64fd25d3ae8dac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005665"
---
# <a name="table-resource-type"></a>Tipo de recurso Table

Representa uma tabela do Excel.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Table](../api/table-get.md) | [WorkbookTable](table.md) |Leia as propriedades e relacionamentos do objeto de tabela.|
|[Create TableColumn](../api/table-post-columns.md) |[WorkbookTableColumn](tablecolumn.md)| Crie uma nova TableColumn postando na coleção de colunas.|
|[List columns](../api/table-list-columns.md) |Coleção [WorkbookTableColumn](tablecolumn.md)| Obtenha uma coleção de objetos TableColumn.|
|[Create TableRow](../api/table-post-rows.md) |[WorkbookTableRow](tablerow.md)| Crie uma nova TableRow postando na coleção de linhas.|
|[List rows](../api/table-list-rows.md) |Coleção [WorkbookTableRow](tablerow.md)| Obtenha uma coleção de objetos TableRow.|
|[Update](../api/table-update.md) | [WorkbookTable](table.md)   |Atualize o objeto Table. |
|[Databodyrange](../api/table-databodyrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado ao corpo de dados da tabela.|
|[Headerrowrange](../api/table-headerrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.|
|[Range](../api/table-range.md)|[Range](range.md)|Obtém o objeto de intervalo associado a toda a tabela.|
|[Totalrowrange](../api/table-totalrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de totais da tabela.|
|[Clearfilters](../api/table-clearfilters.md)|Nenhum|Limpa todos os filtros aplicados à tabela no momento.|
|[Converttorange](../api/table-converttorange.md)|[Range](range.md)|Converte a tabela em um intervalo de células normal. Todos os dados são preservados.|
|[Delete](../api/table-delete.md)|Nenhum|Exclui a tabela.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Nenhum|Aplica novamente todos os filtros à tabela.|
|[List](../api/table-list.md) | Coleção [WorkbookTable](table.md) |Obtenha a coleção de objetos da tabela. |
|[Add](../api/tablecollection-add.md)|[WorkbookTable](table.md)|Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|Retorna um valor que identifica de forma exclusiva a tabela em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.|
|name|string|Nome da tabela.|
|showHeaders|booliano|Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.|
|showTotals|booliano|Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.|
|style|string|Valor de constante que representa o estilo de tabela. Os valores possíveis são: TableStyleLight1 até o TableStyleLight21, TableStyleMedium1 até o TableStyleMedium28, TableStyleStyleDark1 até o TableStyleStyleDark11. Um estilo personalizado de definidas pelo usuário presente na pasta de trabalho também pode ser especificado.|
|highlightFirstColumn|Booliano|Indica se a primeira coluna contém uma formatação especial.   |
|highlightLastColumn|Booliano|Indica se a última coluna contém uma formatação especial. |
|showBandedColumns|Booliano|Indica se as colunas mostram formatação em faixas nas quais as colunas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.   |
|showBandedRows|Booliano|Indica se as linhas mostram formatação em faixas nas quais as linhas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.    |
|showFilterButton|Booliano|Indica se os botões de filtro estão visíveis na parte superior de cada cabeçalho da coluna. Essa configuração só será permitida se a tabela tiver uma linha de cabeçalho.   |
|legacyId|Cadeia de caracteres|ID herdada usada em clientes do Excel anteriores. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columns|Coleção [WorkbookTableColumn](tablecolumn.md)|Representa uma coleção de todas as colunas na tabela. Somente leitura.|
|rows|Coleção [WorkbookTableRow](tablerow.md)|Representa uma coleção de todas as linhas na tabela. Somente leitura.|
|sort|[WorkbookTableSort](tablesort.md)|Representa a classificação da tabela. Somente leitura.|
|planilha|[WorkbookWorksheet](worksheet.md)|A planilha que contém a tabela atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
