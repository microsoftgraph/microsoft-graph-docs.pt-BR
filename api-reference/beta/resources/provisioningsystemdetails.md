---
title: Tipo de recurso provisioningSystemDetails
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5400088c1f239bd73e093679bbc13b8034800f28
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135335"
---
# <a name="provisioningsystemdetails-resource-type"></a>Tipo de recurso provisioningSystemDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o sistema de onde um usuário foi provisionado. Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para o ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é o ServiceNow.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes do sistema.|
|displayName|String|Nome do sistema de onde um usuário foi provisionado.|
|id|String|Identificador do sistema de onde um usuário foi provisionado.|

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


