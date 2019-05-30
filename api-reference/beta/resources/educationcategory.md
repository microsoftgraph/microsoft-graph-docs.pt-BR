---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dd9eccac3a1b6b1bdc3b0eca4c87b5e29e2135a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536170"
---
# <a name="educationcategory-resource-type"></a>tipo de recurso educationCategory

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obter um **educationCategory**existente.|
|[Excluir categoria](../api/educationcategory-delete.md) | Nenhum | Remover um **educationCategory**.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Identificador exclusivo da categoria.|
|displayName|String|Identificador exclusivo da categoria.|

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
