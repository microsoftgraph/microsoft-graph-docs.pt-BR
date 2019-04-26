---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563295"
---
# <a name="provisionedplan-resource-type"></a>Tipo de recurso provisionedPlan

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|capabilityStatus|String|Por exemplo, “Enabled”.|
|provisioningStatus|Cadeia de caracteres|Por exemplo, "Success".|
|service|Cadeia de caracteres|O nome do serviço; por exemplo, "AccessControlS2S".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
