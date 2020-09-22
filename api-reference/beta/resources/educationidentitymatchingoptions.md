---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 73c97b0e9c23c455b3e15ed656060eca7f8a3e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095370"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>tipo de recurso educationIdentityMatchingOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   | Descrição                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| appliesTo          | Cadeia de caracteres | O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`.                                                             |
| sourcePropertyName | Cadeia de caracteres | O nome da propriedade Source, que deve ser um nome de campo nos dados de origem. Essa propriedade diferencia maiúsculas de minúsculas.                                             |
| TargetName | Cadeia de caracteres | O nome da propriedade de destino, que deve ser uma propriedade válida no Azure AD. Essa propriedade diferencia maiúsculas de minúsculas.                                                |
| targetDomain       | Cadeia de caracteres | O domínio a ser sufixo com a propriedade Source para corresponder ao destino. Se fornecido como nulo, a propriedade Source será usada para corresponder à Propriedade Target. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```


