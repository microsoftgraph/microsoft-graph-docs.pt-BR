---
title: tipo de recurso educationIdentityMatchingConfiguration
description: Define as configurações para as identidades correspondentes de perfil de dados da escola. Essas identidades incluem estudantes e professores. Com base nessas configurações, os usuários serão atualizados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: da1c5fa65305e23b8483825103117c523c51edd7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435030"
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
