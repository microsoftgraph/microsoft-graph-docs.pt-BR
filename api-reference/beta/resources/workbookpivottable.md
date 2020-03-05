---
title: tipo de recurso workbookPivotTable
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a086a5f91ad93497b6aa1d841e5baa7ee7e72f96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519201"
---
# <a name="workbookpivottable-resource-type"></a>tipo de recurso workbookPivotTable

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma Tabela Dinâmica do Excel.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |Leia as propriedades e relacionamentos do objeto workbookPivotTable.|
|[Refresh](../api/workbookpivottable-refresh.md)|Nenhum|Atualiza a Tabela Dinâmica. |
|[Refreshall](../api/workbookpivottable-refreshall.md)|Nenhum|Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Id da Tabela Dinâmica.   Somente leitura.|
|name|String|Nome da Tabela Dinâmica.    |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|planilha|[workbookWorksheet](workbookworksheet.md)| A planilha que contém a Tabela Dinâmica atual. Somente leitura.   |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
