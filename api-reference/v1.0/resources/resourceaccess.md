---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 18b1c5b3f42b3f7203363a95b94ed1cf036e7fed
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347994"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

Namespace: microsoft.graph

Objeto usado para especificar um escopo de permissão OAuth 2.0 ou uma função de aplicativo que um aplicativo requer, por meio da propriedade **resourceAccess** do tipo de recurso [requiredResourceAccess](requiredresourceaccess.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo de uma função [de aplicativo](approle.md) ou permissão [delegada](permissionScope.md) exposta pelo aplicativo de recurso. Para permissões delegadas, isso deve corresponder à propriedade **id** de uma das permissões [delegadas](permissionscope.md) na **coleção oauth2PermissionScopes** da entidade de serviço do aplicativo de [recurso](serviceprincipal.md). Para funções de aplicativo (permissões de aplicativo), isso deve corresponder à propriedade **id** de [](approle.md) uma função de aplicativo na coleção **appRoles** da entidade de serviço [do aplicativo de recursos](serviceprincipal.md).|
|type|Cadeia de caracteres|Especifica se a **propriedade id** faz referência a uma [permissão delegada](permissionscope.md) ou a uma função [de aplicativo](approle.md) (permissão de aplicativo). Os valores possíveis são: `Scope` (para permissões delegadas) ou `Role` (para funções de aplicativo).|

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

