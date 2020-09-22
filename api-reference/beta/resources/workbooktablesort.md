---
title: tipo de recurso workbookTableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77f4fb1dcaed54c2b4cd992b7d6105e194812149
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023741"
---
# <a name="workbooktablesort-resource-type"></a>tipo de recurso workbookTableSort

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gerencia operações de classificação em objetos Table.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort-get.md) | [workbookTableSort](workbooktablesort.md) |Leia as propriedades e os relacionamentos do objeto tableSort.|
|[Apply](../api/tablesort-apply.md)|Nenhum|Execute uma operação de classificação.|
|[Clear](../api/tablesort-clear.md)|Nenhum|Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.|
|[Reapply](../api/tablesort-reapply.md)|Nenhum|Reaplica os parâmetros de classificação atuais à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|matchCase|booliano|Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.|
|method|string|Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|campos|[workbookSortField](workbooksortfield.md)|Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


