---
title: tipo de recurso rangeView
description: RangeView representa um conjunto de células visíveis do intervalo pai.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e49392b8a8ef6f79c199d7e7ce7bf2aba22f114
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139419"
---
# <a name="rangeview-resource-type"></a>tipo de recurso rangeView

Namespace: microsoft.graph RangeView representa um conjunto de células visíveis do intervalo pai.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List rows](../api/workbookrangeview-list-rows.md) |Coleção [workbookRangeView](workbookrangeview.md)| Obtenha uma coleção de objetos workbookRangeView.|
|[Itemat](../api/workbookrangeview-itemat.md)|[workbookRangeView](workbookrangeview.md)|Obtenha um item de modo de exibição de intervalo com base no índice.|
|[Range](../api/workbookrangeview-range.md)|[workbookRange](range.md)|Retorna o objeto de intervalo associado à exibição do intervalo|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|cellAddresses|Json|Representa os endereços de célula
|columnCount|Int32|Retorna o número de colunas visíveis. Somente leitura.|
|fórmulas|Json|Representa a fórmula em notação A1. |
|formulasLocal|Json|Representa a fórmula em notação A1, na formatação de número da localidade e no idioma do usuário. Por exemplo, a fórmula "=SUM(A1, 1.5)" em inglês seria "=SOMA(A1; 1,5)" em português.    |
|formulasR1C1|Json|Representa a fórmula em notação no estilo L1C1.   |
|índice|Int32|O índice do intervalo.|
|numberFormat|Json|Representa o código de formato de número do Excel para determinada célula. Somente leitura. |
|rowCount|Int32|Retorna o número de linhas visíveis. Somente leitura.  |
|texto|Json|Valores de texto do intervalo especificado. O valor de texto não depende da largura da célula. A substituição pelo sinal #, que ocorre na interface de usuário do Excel, não afeta o valor de texto retornado pela API. Somente leitura.    |
|valueTypes|Json|Representa o tipo de dados de cada célula. Somente leitura. Os valores possíveis são: Unknown, Empty, String, Integer, Double, Boolean, Error. |
|values|Json|Representa os valores brutos da exibição do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|rows|Coleção [workbookRangeView](workbookrangeview.md)| Representa uma coleção de exibições de tabelas associadas ao intervalo. Somente leitura.    Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```

