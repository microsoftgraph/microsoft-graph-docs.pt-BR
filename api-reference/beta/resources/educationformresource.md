---
title: tipo de recurso educationFormResource
description: Uma subclasse de educationResource. Este recurso é um formulário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f2747d94c80732091db06294b26546afc567e03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334251"
---
# <a name="educationformresource-resource-type"></a>tipo de recurso educationFormResource

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
