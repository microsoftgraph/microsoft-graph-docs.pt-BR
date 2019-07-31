---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6805fabd857e4e906fa095c372632edbcc27fa28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006385"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>tipo de recurso educationIdentityMatchingConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.

> **Observação:** Nenhum usuário é criado quando esse recurso é selecionado.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **matchoptions** | coleção [Microsoft. Graph. educationIdentityMatchingOptions](educationidentitymatchingoptions.md) | Mapeamento entre a conta de usuário e as opções a serem usadas para identificar exclusivamente o usuário a ser atualizado. |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
