---
title: tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status de usuários em seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 2b1a7d2c34ff21c8efd57b358864c4d218630594
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519516"
---
# <a name="userregistrationcount-resource-type"></a>tipo de recurso userRegistrationCount

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a contagem de registro e o status de usuários em seu locatário.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| registrationCount | Int64 | Fornece a contagem de registro para seu locatário. |
| registrationStatus | String | Representa o status do registro do usuário. Os valores possíveis são `registered`: `enabled`, `capable`,, `mfaRegistered`e. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->