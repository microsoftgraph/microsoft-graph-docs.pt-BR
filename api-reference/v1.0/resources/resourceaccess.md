---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 5feb228b1cc29d6a2f608431520cca78591f8b5b
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452654"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

Namespace: microsoft.graph

Objeto usado para especificar um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer, por meio da propriedade **resourceAccess** do tipo de recurso [requiredResourceAccess.](requiredresourceaccess.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|O identificador exclusivo de uma das [instâncias oauth2PermissionScopes](permissionscope.md) ou [appRole](approle.md) que o aplicativo de recurso expõe.|
|type|Cadeia de caracteres|Especifica se a **propriedade id** faz referência a [um oauth2PermissionScopes](permissionscope.md) ou um [appRole](approle.md). Os valores possíveis são: (para escopos de permissão `Scope` OAuth 2.0) ou `Role` (para funções de aplicativo).|

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
  "id": "GUID",
  "type": "String"
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

