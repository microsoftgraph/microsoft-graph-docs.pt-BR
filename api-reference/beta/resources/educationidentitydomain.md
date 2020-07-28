---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4e23a9111d2515234d1aa665f4847d732dc563
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435037"
---
# <a name="educationidentitydomain-resource-type"></a>tipo de recurso educationIdentityDomain

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| appliesTo | Cadeia de caracteres | O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`. |
| nome      | Cadeia de caracteres | Representa o domínio da conta de usuário.                                                        |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```
