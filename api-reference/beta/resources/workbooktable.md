---
title: tipo de recurso workbooktable
description: Representa uma tabela do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1568cc1f08ded8ffdbac04e040bccefe63e9dd02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963882"
---
# <a name="workbooktable-resource-type"></a>tipo de recurso workbooktable

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tabela do Excel.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbooktable](../api/table-get.md) | [workbooktable](workbooktable.md) |Leia as propriedades e relacionamentos do objeto de tabela.|
|[Criar workbookTableColumn](../api/table-post-columns.md) |[workbookTableColumn](workbooktablecolumn.md)| Crie uma nova TableColumn postando na coleção de colunas.|
|[List columns](../api/table-list-columns.md) |coleção [workbookTableColumn](workbooktablecolumn.md)| Obtenha uma coleção de objetos TableColumn.|
|[Criar workbookTableRow](../api/table-post-rows.md) |[workbookTableRow](workbooktablerow.md)| Crie uma nova TableRow postando na coleção de linhas.|
|[List rows](../api/table-list-rows.md) |coleção [workbookTableRow](workbooktablerow.md)| Obtenha uma coleção de objetos TableRow.|
|[Atualizar](../api/table-update.md) | [workbooktable](workbooktable.md)   |Atualize o objeto Table. |
|[Databodyrange](../api/table-databodyrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado ao corpo de dados da tabela.|
|[Headerrowrange](../api/table-headerrowrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.|
|[Range](../api/table-range.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado a toda a tabela.|
|[Totalrowrange](../api/table-totalrowrange.md)|[workbookRange](workbookrange.md)|Obtém o objeto de intervalo associado à linha de totais da tabela.|
|[Clearfilters](../api/table-clearfilters.md)|Nenhum|Limpa todos os filtros aplicados à tabela no momento.|
|[Converttorange](../api/table-converttorange.md)|[workbookRange](workbookrange.md)|Converte a tabela em um intervalo de células normal. Todos os dados são preservados.|
|[Delete](../api/table-delete.md)|None|Exclui a tabela.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Nenhum|Aplica novamente todos os filtros à tabela.|
|[List](../api/table-list.md) | [](workbooktable.md) coleção workbooktable |Obtenha a coleção de objetos da tabela. |
|[Add](../api/tablecollection-add.md)|[workbooktable](workbooktable.md)|Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|Retorna um valor que identifica de forma exclusiva a tabela em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.|
|name|string|Nome da tabela.|
|showHeaders|booliano|Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.|
|showTotals|booliano|Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.|
|style|cadeia de caracteres|Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.|
|highlightFirstColumn|Booliano|Indica se a primeira coluna contém uma formatação especial.   |
|highlightLastColumn|Booliano|Indica se a última coluna contém uma formatação especial. |
|showBandedColumns|Booliano|Indica se as colunas mostram formatação em faixas nas quais as colunas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.   |
|showBandedRows|Booliano|Indica se as linhas mostram formatação em faixas nas quais as linhas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.    |
|showFilterButton|Booliano|Indica se os botões de filtro estão visíveis na parte superior de cada cabeçalho da coluna. Essa configuração só será permitida se a tabela tiver uma linha de cabeçalho.   |
|legacyId|Cadeia de caracteres|ID herdada usada em clientes do Excel anteriores. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columns|coleção [workbookTableColumn](workbooktablecolumn.md)|Representa uma coleção de todas as colunas na tabela. Somente leitura.|
|rows|coleção [workbookTableRow](workbooktablerow.md)|Representa uma coleção de todas as linhas na tabela. Somente leitura.|
|sort|[workbookTableSort](workbooktablesort.md)|Representa a classificação da tabela. Somente leitura.|
|planilha|[workbookWorksheet](workbookworksheet.md)|A planilha que contém a tabela atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
