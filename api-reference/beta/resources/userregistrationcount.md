---
title: Tipo de recurso userRegistrationCount
description: Representa a contagem de registro e o status dos usuários em seu locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5cdcdb4cfd56c0828cfeb7e71defe4c7459e3133
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132948"
---
# <a name="userregistrationcount-resource-type"></a>Tipo de recurso userRegistrationCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a contagem de registro e o status dos usuários em seu locatário.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| registrationCount | Int64 | Fornece a contagem de registro para seu locatário. |
| registrationStatus | String | Representa o status do registro do usuário. Os valores possíveis `registered` são: `enabled` , e `capable` `mfaRegistered` . |

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

