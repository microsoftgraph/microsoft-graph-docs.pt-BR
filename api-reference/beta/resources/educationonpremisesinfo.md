---
title: tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764731"
---
# <a name="educationonpremisesinfo-resource-type"></a>tipo de recurso educationOnPremisesInfo

Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| imutávelid | String | Identificador exclusivo do objeto de usuário no Active Directory. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
