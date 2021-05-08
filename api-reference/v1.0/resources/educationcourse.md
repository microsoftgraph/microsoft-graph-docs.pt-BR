---
title: Tipo de recurso educationCourse
description: Representa as informações do curso para uma classe.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232121"
---
# <a name="educationcourse-resource-type"></a>Tipo de recurso educationCourse

Namespace: microsoft.graph

Representa as informações do curso para uma classe. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | Identificador exclusivo do curso.         |
| descrição  | String | Descrição do curso.                |
| displayName  | String | Nome do curso.                       |
| externalId   | Cadeia de caracteres | ID do curso do sistema de sincronização. |
| Assunto      | String | Assunto do curso.                    |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
