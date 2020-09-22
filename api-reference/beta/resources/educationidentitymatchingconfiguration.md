---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7c26ef1447272b88c59ec6992e41ae051439645e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095386"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a>tipo de recurso educationIdentityMatchingConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.

> [!NOTE]
> Nenhum usuário é criado quando esse recurso é selecionado.

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo                                                                                               | Descrição                                                                                      |
| :-------------- | :------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| matchoptions | coleção [Microsoft. Graph. educationIdentityMatchingOptions](educationidentitymatchingoptions.md) | Mapeamento entre a conta de usuário e as opções a serem usadas para identificar exclusivamente o usuário a ser atualizado. |

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
      "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```


