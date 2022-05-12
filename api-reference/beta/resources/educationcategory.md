---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 49e5f0c27cb643cdba94dc710ae980ef946d19d1
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366104"
---
# <a name="educationcategory-resource-type"></a>Tipo de recurso educationCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma categoria que pode ser aplicada a atribuições.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Crie uma **nova educationCategory**.|
|[Obter educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Obtenha uma **educationCategory existente**.|
|[Excluir categoria](../api/educationcategory-delete.md) | Nenhuma | Remover uma **educationCategory**.|
|[Obter delta](../api/educationcategory-delta.md)|[coleção educationCategory](../resources/educationcategory.md)|Obtenha uma lista de **educationCategory** recém-criada ou atualizada sem precisar executar uma leitura completa da coleção.|


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
