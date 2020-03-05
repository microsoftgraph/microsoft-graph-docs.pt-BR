---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a21d4d3005be8a776ae8bb9f9e3c1027be48de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501924"
---
# <a name="educationidentitydomain-resource-type"></a>tipo de recurso educationIdentityDomain

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md). 

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string |  O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`.      |
| **name** | string |  Representa o domínio da conta de usuário.         |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
