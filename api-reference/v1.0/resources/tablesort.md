---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be607832be82b99853b4cd44cfa5b60449a2c432
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929470"
---
# <a name="tablesort-resource-type"></a>Tipo de recurso TableSort

Gerencia operações de classificação em objetos Table.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |Leia as propriedades e os relacionamentos do objeto tableSort.|
|[Aplicar](../api/tablesort-apply.md)|Nenhum|Execute uma operação de classificação.|
|[Clear](../api/tablesort-clear.md)|Nenhum|Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.|
|[Reapply](../api/tablesort-reapply.md)|Nenhum|Reaplica os parâmetros de classificação atuais à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|campos|Coleção [WorkbookSortField](sortfield.md)|Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.|
|matchCase|booliano|Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.|
|method|string|Representa caracteres do chinês método última usado para classificar a tabela de pedidos. Os valores possíveis são: `PinYin`, `StrokeCount`. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
