---
title: Tipo de recurso educationStudent
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407057446753afc0cf8f9f63ebbf4459c4106f8ec1dbcc9c49844a93e69b2388
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238115"
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
