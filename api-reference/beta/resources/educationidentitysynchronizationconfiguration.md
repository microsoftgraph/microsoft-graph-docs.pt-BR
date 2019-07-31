---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972674"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>tipo de recurso educationIdentitySynchronizationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD). |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Use este tipo para criar novas contas de usuário no Azure AD. |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

