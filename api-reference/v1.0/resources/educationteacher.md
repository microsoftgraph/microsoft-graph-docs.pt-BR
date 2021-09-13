---
title: Tipo de recurso educationTeacher
description: Informações adicionais incluídas a um educationUser que está presente quando a primaryRole de um usuário é `teacher`.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 68c6cde2b3e7027e94c9d1ce818eea46778b5d6c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118684"
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
