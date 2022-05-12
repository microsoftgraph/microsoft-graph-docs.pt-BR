---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2a265a8733b72dc26967b390503abdbf201d9a1e
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65365908"
---
# <a name="educationcategory-resource-type"></a>Tipo de recurso educationCategory

Namespace: microsoft.graph

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Crie uma **nova educationCategory**.|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obtenha uma **educationCategory existente**.|
|[Excluir categoria](../api/educationcategory-delete.md) | Nenhuma | Remover uma **educationCategory**.|
|[Obter delta](../api/educationcategory-delta.md)|[coleção educationCategory](../resources/educationcategory.md)|Obtenha uma lista de objetos **educationCategory** recém-criados ou atualizados sem precisar executar uma leitura completa da coleção.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Identificador exclusivo para a categoria.|
|displayName|Cadeia de caracteres|Identificador exclusivo para a categoria.|

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


