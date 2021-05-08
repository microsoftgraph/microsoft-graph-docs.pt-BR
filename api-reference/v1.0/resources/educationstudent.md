---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231847"
---
# <a name="educationstudent-resource-type"></a>Tipo de recurso educationStudent

Namespace: microsoft.graph

Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `student`.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo            | Descrição                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| birthDate      | Data            | Data de nascimento do aluno.                                                |
| externalId     | Cadeia de caracteres          | ID do aluno no sistema de origem.                                   |
| gender         | educationGender | Os valores possíveis são: `female`, `male`, `other`, `unknownFutureValue`. |
| grade          | Cadeia de caracteres          | Nível de classificação atual do aluno.                                       |
| graduationYear | Cadeia de caracteres          | Ano que o aluno está graduando na escola.                           |
| studentNumber  | Cadeia de caracteres          | Número do aluno.                                                           |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
