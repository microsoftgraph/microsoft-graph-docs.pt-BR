---
title: Tipo de recurso Worksheet
description: Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.
ms.openlocfilehash: 513a1fceb8e0b7e2c7667d5fac2e4a5978ed7c04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034135"
---
# <a name="worksheet-resource-type"></a>Tipo de recurso Worksheet

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Worksheet](../api/worksheet-get.md) | [Worksheet](worksheet.md) |Leia as propriedades e os relacionamentos do objeto de planilha.|
|[Create Chart](../api/worksheet-post-charts.md) |[Chart](chart.md)| Crie um novo Gráfico ao postar na coleção de gráficos.|
|[Nomes da lista](../api/worksheet-list-names.md) |Coleção [NamedItem](nameditem.md)| Faça com que a coleção de itens nomeados seja associada à planilha.|
|[Listar gráficos](../api/worksheet-list-charts.md) |Coleção [Chart](chart.md)| Obtenha a coleção de objetos Chart.|
|[Create Table](../api/worksheet-post-tables.md) |[Table](table.md)| Crie uma nova Table postando na coleção de tabelas.|
|[List tables](../api/worksheet-list-tables.md) |Coleção [Table](table.md)| Obtenha uma coleção de objetos Table.|
|[Update](../api/worksheet-update.md) | [Worksheet](worksheet.md)   |Atualize o objeto Worksheet. |
|[Cell](../api/worksheet-cell.md)|[Range](range.md)|Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.|
|[Range](../api/worksheet-range.md)|[Range](range.md)|Obtém o objeto de intervalo especificado pelo nome ou endereço.|
|[Usedrange](../api/worksheet-usedrange.md)|[Range](range.md)|O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.|
|[Delete](../api/worksheet-delete.md)|Nenhum|Exclui a planilha da pasta de trabalho.|
|[List](../api/worksheet-list.md) | Coleção [Worksheet](worksheet.md) |Obtenha a coleção de objetos da planilha. |
|[Add](../api/worksheetcollection-add.md)|[Worksheet](worksheet.md)|Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. |
|[List pivotTables](../api/workbookworksheet-list-pivottables.md) |Coleção [workbookPivotTable](workbookpivottable.md)| Obtenha uma coleção de objeto workbookPivotTable.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.|
|name|string|O nome de exibição da planilha.|
|position|inteiro|A posição baseada em zero da planilha na pasta de trabalho.|
|visibilidade|string|A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|charts|Coleção [Chart](chart.md)|Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.|
|names|Coleção [NamedItem](nameditem.md)|Retorna a coleção de nomes associados à planilha. Somente leitura.|
|pivotTables|Coleção [workbookPivotTable](workbookpivottable.md)| Coleção de Tabelas Dinâmicas que fazem parte da planilha. |
|protection|[WorksheetProtection](worksheetprotection.md)|Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.|
|tables|Coleção [Table](table.md)|Coleção de tabelas que fazem parte da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
