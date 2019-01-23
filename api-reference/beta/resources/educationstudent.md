---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ce3e28ccedc5f6165c8c333afb2ccd10343f14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406903"
---
# <a name="educationstudent-resource-type"></a>Tipo de recurso educationStudent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|birthDate|Data| Data de nascimento do aluno.|
|externalId|Cadeia de caracteres| ID do aluno no sistema de origem.|
|gender|educationGender| Os valores possíveis são: `female`, `male`, `other`, `unkownFutureValue`.|
|grade|Cadeia de caracteres|Nível de classificação atual do aluno.|
|graduationYear|Cadeia de caracteres| Ano que o aluno está graduando na escola.|
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
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
