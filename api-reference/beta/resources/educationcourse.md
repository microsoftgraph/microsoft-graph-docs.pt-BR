---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eac609f787621e30d4707d477296fc53af77dad0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764729"
---
# <a name="educationcourse-resource-type"></a>tipo de recurso educationCourse

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de curso de uma aula. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | Identificador exclusivo do curso.         |
| descrição  | String | Descrição do curso.                |
| displayName  | String | Nome do curso.                       |
| externalId   | Cadeia de caracteres | ID do curso do sistema de sincronização. |
| subject      | Cadeia de caracteres | Assunto do curso.                    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
