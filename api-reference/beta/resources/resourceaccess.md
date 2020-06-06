---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 6092a427a2882c4b6bdae07bb98f8bc8a81eecfb
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2020
ms.locfileid: "44593629"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo. A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo de uma das instâncias [oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.|
|tipo|String|Especifica se a propriedade **ID** faz referência a um [Oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md). Os valores possíveis são `Scope` ou `Role` .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
