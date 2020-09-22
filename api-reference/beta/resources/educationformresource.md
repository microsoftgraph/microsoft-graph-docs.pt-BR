---
title: tipo de recurso educationFormResource
description: Uma subclasse de educationResource. Este recurso é um formulário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0c8748c725f7289eadbca8119b47bf8a81b28c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095434"
---
# <a name="educationformresource-resource-type"></a>tipo de recurso educationFormResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationResource](educationresource.md). Este recurso é um formulário.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|originalFormId|Cadeia de caracteres|ID original do formulário.|
|formId|Cadeia de caracteres|ID do formulário.|
|isGroupForm|Boolean|Se o formulário pertence a um grupo de classe.|
|viewUrl|Cadeia de caracteres|URL do aluno para o formulário.|
|viewUrl|Cadeia de caracteres|URL do aluno para o formulário.|
|editUrl|Cadeia de caracteres|URL do professor para o formulário.|

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


