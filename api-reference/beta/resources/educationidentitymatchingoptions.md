---
title: tipo de recurso de educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de fonte e uma propriedade de destino para contas de usuário correspondentes. A propriedade source deve existir nos dados de origem. A propriedade de destino deve ser uma propriedade válida, no Windows Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425789"
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
