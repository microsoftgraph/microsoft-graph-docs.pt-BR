---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1ffa1bbcd3f96c86818c68d350236086d0975187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501791"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>tipo de recurso educationIdentitySynchronizationConfiguration

Namespace: Microsoft. Graph

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

