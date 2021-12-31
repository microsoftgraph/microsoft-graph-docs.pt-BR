---
title: Tipo de recurso auditActivityInitiator
description: Identidade do objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: e681f56f3caf0792241a92ce5137ac8468b623d8
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647159"
---
# <a name="auditactivityinitiator-resource-type"></a>Tipo de recurso auditActivityInitiator

Namespace: microsoft.graph Identity o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aplicativo|[appIdentity](appidentity.md)|Se o ator que inicia a atividade for um aplicativo, essa propriedade indicará todas as suas informações de identificação, incluindo appId, displayName, servicePrincipalId e servicePrincipalName.|
|usuário|[auditUserIdentity](auditUserIdentity.md)|Se o ator que inicia a atividade for um usuário, essa propriedade indicará suas informações de identificação, incluindo sua id, displayName e userPrincipalName.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


