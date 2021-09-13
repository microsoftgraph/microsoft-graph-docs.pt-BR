---
title: Tipo de recurso educationCourse
description: Representa as informações do curso para uma classe.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b0345e6be308a175fbb14ab618fcf66564f45f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036708"
---
# <a name="educationcourse-resource-type"></a>Tipo de recurso educationCourse

Namespace: microsoft.graph

Representa as informações do curso para uma classe. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | Cadeia de caracteres | Identificador exclusivo do curso.         |
| description  | String | Descrição do curso.                |
| displayName  | Cadeia de caracteres | Nome do curso.                       |
| externalId   | Cadeia de caracteres | ID do curso do sistema de sincronização. |
| assunto      | Cadeia de caracteres | Assunto do curso.                    |

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
