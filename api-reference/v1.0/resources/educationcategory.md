---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b8454265c7c01b7e9a27653e06e0d383d0e7f944f451adc55e5688faecaa79a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130363"
---
# <a name="educationcategory-resource-type"></a>Tipo de recurso educationCategory

Namespace: microsoft.graph

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Criar uma nova **educationCategory**.|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obter uma **educationCategory existente**.|
|[Excluir categoria](../api/educationcategory-delete.md) | None | Remover uma **educationCategory**.|


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
  "id": "String (identifier)",
  "displayName": "String",
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


