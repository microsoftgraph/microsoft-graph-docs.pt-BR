---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c96e3301966f4089df2f973d4e8906b9fb010ffb2f9cd2eda81c8c543395ff2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141732"
---
# <a name="teacher-resource-type"></a>Tipo de recurso professor

Namespace: microsoft.graph

Informações adicionais incluídas a um [educationUser](educationuser.md) que está presente quando a primaryRole de um usuário é `teacher`.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo   | Descrição                             |
| :------------ | :----- | :-------------------------------------- |
| externalId    | Cadeia de caracteres | ID do professor no sistema de origem. |
| teacherNumber | Cadeia de caracteres | Número do professor.                         |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTeacher"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTeacher",
  "teacherNumber": "String",
  "externalId": "String"
}
```
