---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 15c6427062f09493168f0f94cca3060bc3f631de
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390882"
---
# <a name="educationcategory-resource-type"></a>Tipo de recurso educationCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Criar uma nova **educationCategory**.|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obter uma **educationCategory existente**.|
|[Excluir categoria](../api/educationcategory-delete.md) | Nenhum | Remover uma **educationCategory**.|
|[Obter delta](../api/educationcategory-delta.md)|[Coleção educationCategory](../resources/educationcategory.md)|Obter uma lista de **objetos educationCategory** que pertencem a essa classe com suporte à consulta delta.|


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


