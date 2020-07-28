---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435016"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>tipo de recurso educationIdentitySynchronizationConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.

## <a name="derived-types"></a>Tipos derivados

| Tipo                                                                                | Descrição                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) | Use este tipo para **fazer a correspondência** de contas de usuário existentes no Azure Active Directory. |
| [educationIdentityCreationConfiguration](educationidentitycreationconfiguration.md) | Use este tipo para **criar novas** contas de usuário no Azure Active Directory.                              |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```
