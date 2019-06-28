---
title: tipo de recurso provisioningSystemDetails
description: Representa o sistema do qual um usuário foi provisionado ou de.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349327"
---
# <a name="provisioningsystemdetails-resource-type"></a>tipo de recurso provisioningSystemDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o sistema do qual um usuário foi provisionado ou de. Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes do sistema.|
|displayName|String|Nome do sistema no qual um usuário foi provisionado ou de.|
|id|String|Identificador do sistema no qual um usuário foi provisionado ou de.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
