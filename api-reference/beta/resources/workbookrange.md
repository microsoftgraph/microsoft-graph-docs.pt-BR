---
title: tipo de recurso workbookRange
description: Range representa um conjunto de uma ou mais células contíguas, como uma célula, uma linha, uma coluna, um bloco de células, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b0f4afa72c4662f3f1254371a2c0170792a14196
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046213"
---
# <a name="workbookrange-resource-type"></a>tipo de recurso workbookRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Range representa um conjunto de uma ou mais células contíguas, como uma célula, uma linha, uma coluna, um bloco de células, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Range](../api/range-get.md) | [workbookRange](workbookrange.md) |Leia as propriedades e relacionamentos do objeto de intervalo.|
|[Update](../api/range-update.md) | [workbookRange](workbookrange.md)   |Atualize o objeto Range. |
|[Boundingrect](../api/range-boundingrect.md)|[workbookRange](workbookrange.md)|Obtém o menor objeto de intervalo que abrange os intervalos determinados. Por exemplo, GetBoundingRect de "B2:C5" e "D10:E15" é "B2:E16".|
|[Cell](../api/range-cell.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha. A localização da célula retornada está relacionada à célula superior esquerda do intervalo.|
|[Column](../api/range-column.md)|[workbookRange](workbookrange.md)|Obtém uma coluna incluída no intervalo.|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|Obtém um determinado número de colunas à direita do intervalo especificado.|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|Obtém um determinado número de colunas à esquerda do intervalo especificado.|
|[Entirecolumn](../api/range-entirecolumn.md)|[workbookRange](workbookrange.md)|Obtém um objeto que representa toda a coluna do intervalo.|
|[Entirerow](../api/range-entirerow.md)|[workbookRange](workbookrange.md)|Obtém um objeto que representa toda a linha do intervalo.|
|[Intersection](../api/range-intersection.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.|
|[Lastcell](../api/range-lastcell.md)|[Range](workbookrange.md)|Obtém a última célula do intervalo. Por exemplo, a última célula de "B2:D5" é "D5".|
|[Lastcolumn](../api/range-lastcolumn.md)|[workbookRange](workbookrange.md)|Obtém a última coluna do intervalo. Por exemplo, a última coluna de "B2:D5" é "D2:D5".|
|[Lastrow](../api/range-lastrow.md)|[Range](workbookrange.md)|Obtém a última linha do intervalo. Por exemplo, a última linha de "B2:D5" é "B5:D5".|
|[Offsetrange](../api/range-offsetrange.md)|[workbookRange](workbookrange.md)|Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.|
|[Row](../api/range-row.md)|[Range](workbookrange.md)|Obtém uma linha contida no intervalo.|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|Obtém um determinado número de linhas acima de um determinado intervalo.|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|Obtém um determinado número de linhas abaixo de um determinado intervalo.|
|[Usedrange](../api/range-usedrange.md)|[workbookRange](workbookrange.md)|Retorna o intervalo usado do objeto de intervalo determinado.|
|[Clear](../api/range-clear.md)|Nenhum|Limpe valores de intervalo, formatação, preenchimento, bordas, etc.|
|[Delete](../api/range-delete.md)|Nenhum|Exclui as células associadas ao intervalo.|
|[Insert](../api/range-insert.md)|[workbookRange](workbookrange.md)|Insere uma célula ou um intervalo de células na planilha, no lugar desse intervalo, e desloca as outras células para liberar espaço. Retorna um novo objeto Range no espaço em branco atual.|
|[Merge](../api/range-merge.md)|Nenhum|Mescla as células do intervalo em uma região da planilha.|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.|
|[Unmerge](../api/range-unmerge.md)|Nenhum|Desfaz a mesclagem das células do intervalo em células separadas.|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|Obtenha o intervalo visível de um intervalo filtrado.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|cadeia de caracteres|Representa a referência do intervalo no estilo A1. O valor do endereço inclui a referência de planilha (por exemplo, Plan1!A1:B4). Somente leitura.|
|addressLocal|string|Representa a referência de intervalo para o intervalo especificado no idioma do usuário. Somente leitura.|
|cellCount|int|Número de células no intervalo. Somente leitura.|
|columnCount|int|Representa o número total de colunas no intervalo. Somente leitura.|
|columnHidden|booliano|Representa se todas as colunas do intervalo atual estão ocultas.|
|columnIndex|int|Representa o número de colunas da primeira célula no intervalo. Indexados com zero. Somente leitura.|
|fórmulas|Json|Representa a fórmula em notação A1.|
|formulasLocal|Json|Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário.  Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.|
|formulasR1C1|Json|Representa a fórmula em notação no estilo L1C1.|
|hidden|booliano|Representa se todas as células do intervalo atual estão ocultas. Somente leitura.|
|numberFormat|Json|Representa o código de formato de número do Excel para determinada célula.|
|rowCount|int|Retorna o número total de linhas no intervalo. Somente leitura.|
|rowHidden|booliano|Representa se todas as linhas do intervalo atual estão ocultas.|
|rowIndex|int|Representa o número de linhas da primeira célula no intervalo. Indexados com zero. Somente leitura.|
|texto|Json|Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.|
|valueTypes|cadeia de caracteres|Representa o tipo de dados de cada célula. Os valores possíveis são: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean` e `Error`. Somente leitura.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookRangeFormat](workbookrangeformat.md)|Retorna um objeto de formato que encapsula a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo. Somente leitura.|
|sort|[workbookRangeSort](workbookrangesort.md)|A planilha que contém o intervalo atual. Somente leitura.|
|planilha|[workbookWorksheet](workbookworksheet.md)|A planilha que contém o intervalo atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRange"
}-->

```json
{
  "id": "string",
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "hidden": true,
  "numberFormat": "Json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "Json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


