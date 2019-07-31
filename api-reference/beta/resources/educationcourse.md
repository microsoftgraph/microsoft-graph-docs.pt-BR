---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c160f9bd20f7dfccfa19dbf4d466dd967fde9c2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972758"
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
