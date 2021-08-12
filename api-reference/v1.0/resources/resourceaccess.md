---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0d5c8a60b1080b1e605dde754d8007cf15b36b129d276a6b2d9f87421ba9ef25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243306"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

Namespace: microsoft.graph

Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer. A **propriedade resourceAccess** do [tipo requiredResourceAccess](requiredresourceaccess.md) é uma coleção **de ResourceAccess**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo de uma das [instâncias oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recurso expõe.|
|tipo|Cadeia de caracteres|Especifica se a **propriedade id** faz referência a [um oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md). Os valores possíveis são: `Scope` ou `Role`.|

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

