---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86e65d46c8037ebcbb2c98f9f9e93f94f34bbdef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972702"
---
# <a name="educationidentitydomain-resource-type"></a>tipo de recurso educationIdentityDomain

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
