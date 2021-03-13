---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: bad89764571b6ab3a2770432a950428fec0d9407
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761301"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

Namespace: microsoft.graph

Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer. A **propriedade resourceAccess** do [tipo requiredResourceAccess](requiredresourceaccess.md) é uma coleção **de ResourceAccess**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo de uma das [instâncias oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recurso expõe.|
|tipo|String|Especifica se a **propriedade id** faz referência a [um oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md). Os valores possíveis são: `Scope` ou `Role`.|

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

