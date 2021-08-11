---
title: Tipo de recurso educationCourse
description: Representa as informações do curso para uma classe.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e54870ad3633f0b0170a54fad32ce8aa0baa2843466dd0f0e051caeacca54ffa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135250"
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
| Assunto      | Cadeia de caracteres | Assunto do curso.                    |

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
