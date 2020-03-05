---
title: tipo de recurso educationCourse
description: Representa as informações de curso de uma aula.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ba29e98150db6ffa9938585540d9b77f8a755cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502267"
---
# <a name="educationcourse-resource-type"></a>tipo de recurso educationCourse

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de curso de uma aula. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | Identificador exclusivo do curso.         |
| description  | String | Descrição do curso.                |
| displayName  | Cadeia de caracteres | Nome do curso.                       |
| externalId   | String | ID do curso do sistema de sincronização. |
| assunto      | String | Assunto do curso.                    |

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
