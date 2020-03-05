---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9b8f2de9f3b40a72aab7f9273b9b4fc30594059b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500762"
---
# <a name="educationstudent-resource-type"></a>Tipo de recurso educationStudent

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|birthDate|Data| Data de nascimento do aluno.|
|externalId|String| ID do aluno no sistema de origem.|
|gender|educationGender| Os valores possíveis são: `female`, `male`, `other`.|
|grade|String|Nível de classificação atual do aluno.|
|graduationYear|String| Ano que o aluno está graduando na escola.|
|studentNumber|Cadeia de caracteres| Número do aluno.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
