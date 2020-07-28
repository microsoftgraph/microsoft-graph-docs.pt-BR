---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b17ca8548d7a70b8f652ad2d54455fb6040677d
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435023"
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
