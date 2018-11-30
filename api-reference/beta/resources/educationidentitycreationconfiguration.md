---
title: tipo de recurso de educationIdentityCreationConfiguration
description: Define as configurações na criação das identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão criados no diretório.
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040159"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>tipo de recurso de educationIdentityCreationConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define as configurações na criação das identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão criados no diretório.

> **Observação:** Se você tiver ativada a sincronização entre o local do Active Directory e o Azure Active Directory (AD Azure) de sincronização de diretório, use o recurso de [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) .

Derivado do [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **userDomains** | coleção [educationIdentityDomain](educationidentitydomain.md) |  Define a lista de domínios a serem utilizadas por tipo de usuário.  |


## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```