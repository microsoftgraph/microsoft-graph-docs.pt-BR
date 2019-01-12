---
title: tipo de recurso de educationIdentityMatchingConfiguration
description: Define as configurações para a correspondência de identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ee9f58c2f69882361ee105a1d7531bb5756e165
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977546"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>tipo de recurso de educationIdentityMatchingConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define as configurações para a correspondência de identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão atualizados no diretório.

> **Observação:** Nenhum usuário é criado quando este recurso for selecionado.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **matchingOptions** | coleção [educationIdentityMatchingOptions](educationidentitymatchingoptions.md) | Mapeamento entre a conta de usuário e as opções utilizado para identificar exclusivamente o usuário a ser atualizado. |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
