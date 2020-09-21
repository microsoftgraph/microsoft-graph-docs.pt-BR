---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2eae690076553090dbd32f46f0b777a998b615d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979536"
---
# <a name="educationteacher-resource-type"></a>Tipo de recurso educationTeacher

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.

> [!IMPORTANT]
> Ao usar escopos de permissão delegada, o Graph retornará apenas as `externalId` Propriedades. Todas as outras propriedades exigem escopos de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                                  |
| :------------ | :----- | :------------------------------------------- |
| externalId    | Cadeia de caracteres | ID do professor no sistema de origem externo. |
| teacherNumber | Cadeia de caracteres | Número do professor.                              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


