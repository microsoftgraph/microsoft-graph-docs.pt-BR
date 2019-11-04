---
title: tipo de recurso relatedPerson
description: tipo de recurso relatedPerson
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6be6300bc901305fb87b04e2482f145b9187f9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939233"
---
# <a name="relatedperson-resource-type"></a>tipo de recurso relatedPerson

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre as pessoas relacionadas às informações de uma determinada entidade em um [perfil](profile.md) de um usuário.

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo        | Descrição                                               |
|:----------------|:------------|:----------------------------------------------------------|
|displayName      |Cadeia de caracteres       | Nome da pessoa.                                        |
|relação     |String       | Os valores possíveis são: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.|
|userPrincipalName|String       | Endereço de email ou referência a uma pessoa na organização. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
