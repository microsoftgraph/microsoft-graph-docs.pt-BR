---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d722beaac54cbd57c227457a0883b856f6eca4bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501826"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>tipo de recurso educationIdentityMatchingOptions

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string |  O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`.      |
| **sourcePropertyName** | string |  O nome da propriedade Source, que deve ser um nome de campo nos dados de origem. Essa propriedade diferencia maiúsculas de minúsculas.        |
| **TargetName** | string |  O nome da propriedade de destino, que deve ser uma propriedade válida no Azure AD. Essa propriedade diferencia maiúsculas de minúsculas.     |
| **targetDomain** | string |  O domínio a ser sufixo com a propriedade Source para corresponder ao destino. Se fornecido como nulo, a propriedade Source será usada para corresponder à Propriedade Target.        |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
