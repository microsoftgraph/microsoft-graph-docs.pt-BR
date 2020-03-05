---
title: tipo de recurso educationFormResource
description: Uma subclasse de educationResource. Este recurso é um formulário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ed81e1e9e74ad311e4102963649ff4a4015bb093
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501959"
---
# <a name="educationformresource-resource-type"></a>tipo de recurso educationFormResource

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationResource](educationresource.md). Este recurso é um formulário.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|originalFormId|String|ID original do formulário.|
|formId|String|ID do formulário.|
|isGroupForm|Boolean|Se o formulário pertence a um grupo de classe.|
|viewUrl|String|URL do aluno para o formulário.|
|viewUrl|String|URL do aluno para o formulário.|
|editUrl|String|URL do professor para o formulário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
