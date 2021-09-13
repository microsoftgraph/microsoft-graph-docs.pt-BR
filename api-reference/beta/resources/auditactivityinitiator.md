---
title: Tipo de recurso auditActivityInitiator
description: Identidade do objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: a018a6e74f9ee89b879577bec6f64a94ab15cdca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047482"
---
# <a name="auditactivityinitiator-resource-type"></a>Tipo de recurso auditActivityInitiator

Namespace: microsoft.graph Identity o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aplicativo|[appIdentity](appidentity.md)|Se o recurso que inicia a atividade for um aplicativo, essa propriedade indicará todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalId, Name.|
|usuário|[userIdentity](useridentity.md)|Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.|

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


