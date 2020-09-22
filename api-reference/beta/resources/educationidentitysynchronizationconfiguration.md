---
title: tipo de recurso educationIdentitySynchronizationConfiguration
description: Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e193c798f1f3fbc5d4d1c9d8c7b96eed7d39cf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095356"
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


