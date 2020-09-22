---
title: tipo de recurso educationIdentityCreationConfiguration
description: Define as configurações de criação de identidades de perfis de dados escolares. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4dc03514e3d62f0dca096b0e669ada9247ff39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095398"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a>tipo de recurso educationIdentityCreationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as configurações de criação de identidades de perfis de dados escolares. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão criados no diretório.

> [!WARNING]
> Se você tiver a sincronização de diretório ativada para sincronizar entre o Active Directory local e o Azure Active Directory (Azure AD), use o recurso [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) em vez disso.

Derivado de [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                                                             | Descrição                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| userdomains | coleção [educationIdentityDomain](educationidentitydomain.md) | Define a lista de domínios a serem usados por tipo de usuário. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```


