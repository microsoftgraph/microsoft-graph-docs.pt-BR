---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82ad4f009ca76625c148e8a42e58385195466fbb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095538"
---
# <a name="educationcategory-resource-type"></a>tipo de recurso educationCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Criar um novo **educationCategory**.|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obter um **educationCategory**existente.|
|[Excluir categoria](../api/educationcategory-delete.md) | Nenhum | Remover um **educationCategory**.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Identificador exclusivo da categoria.|
|displayName|Cadeia de caracteres|Identificador exclusivo da categoria.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


