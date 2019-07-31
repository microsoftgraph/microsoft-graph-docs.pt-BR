---
title: tipo de recurso auditActivityInitiator
description: Identity o objeto Resource que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f76c071efd10d2d43887bdd5dd04df0d2aa86d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974224"
---
# <a name="auditactivityinitiator-resource-type"></a>tipo de recurso auditActivityInitiator
Identity o objeto Resource que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aplicativo|[appIdentity](appidentity.md)|Se o recurso que inicia a atividade for um aplicativo, essa propriedade indica todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalName, Name.|
|user|[userIdentity](useridentity.md)|Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.|

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
