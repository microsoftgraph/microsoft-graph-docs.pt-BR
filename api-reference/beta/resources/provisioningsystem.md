---
title: Tipo de recurso provisioningSystem
description: Representa o sistema de onde um usuário foi provisionado.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2dcc52e4b847648477313d61c8b69b168a8807b1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232900"
---
# <a name="provisioningsystem-resource-type"></a>Tipo de recurso provisioningSystem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o sistema de onde um usuário foi provisionado. Por exemplo, ao provisionar um usuário do Azure Active Directory (Azure AD) para ServiceNow, o sistema de origem é o Azure AD e o sistema de destino é ServiceNow.

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
  "@odata.type": "microsoft.graph.provisioningSystem",
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
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


