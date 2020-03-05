---
title: tipo de recurso relatedPerson
description: tipo de recurso relatedPerson
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 507746674f17a7bf8255ccddc53ea14fe2ca5a26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521177"
---
# <a name="relatedperson-resource-type"></a>tipo de recurso relatedPerson

Namespace: Microsoft. Graph

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
