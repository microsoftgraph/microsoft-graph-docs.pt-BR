---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
ms.openlocfilehash: 2cabb255648f4089d437912a97bb7d29ff286779
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038546"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>tipo de recurso de educationIdentityMatchingOptions

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string |  O tipo de função de usuário para atribuir da licença. Os valores possíveis são: `student` e `teacher`.      |
| **sourcePropertyName** | string |  O nome da propriedade source, que deve ser um nome de campo nos dados de origem. Essa propriedade diferencia maiusculas de minúsculas.        |
| **targetPropertyName** | string |  O nome da propriedade destino, que deve ser uma propriedade válida no Azure AD. Essa propriedade diferencia maiusculas de minúsculas.     |
| **targetDomain** | string |  O domínio ao sufixo com a propriedade source a correspondência de destino. Caso seja fornecido como nulo, a propriedade source será usada para coincidir com a propriedade de destino.        |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
