---
title: tipo de recurso provisioningSystemDetails
description: Representa o sistema do qual um usuário foi provisionado ou de.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 286ae448cbbaee428820d274d11d8584a9150393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521317"
---
# <a name="provisioningsystemdetails-resource-type"></a>tipo de recurso provisioningSystemDetails

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o sistema do qual um usuário foi provisionado ou de. Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes do sistema.|
|displayName|Cadeia de caracteres|Nome do sistema no qual um usuário foi provisionado ou de.|
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
