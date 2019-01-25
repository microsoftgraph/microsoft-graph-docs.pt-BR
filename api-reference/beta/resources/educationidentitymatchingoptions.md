---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513701"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>tipo de recurso de educationIdentityMatchingOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| appliesTo | string |  O tipo de função de usuário para atribuir da licença. Os valores possíveis são: `student` e `teacher`.      |
| **sourcePropertyName** | string |  O nome da propriedade source, que deve ser um nome de campo nos dados de origem. Essa propriedade diferencia maiusculas de minúsculas.        |
| **targetPropertyName** | string |  O nome da propriedade destino, que deve ser uma propriedade válida no Azure AD. Essa propriedade diferencia maiusculas de minúsculas.     |
| **targetDomain** | string |  O domínio ao sufixo com a propriedade source a correspondência de destino. Caso seja fornecido como nulo, a propriedade source será usada para coincidir com a propriedade de destino.        |

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
