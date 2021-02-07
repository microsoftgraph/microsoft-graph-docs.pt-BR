---
title: Tipo de recurso auditActivityInitiator
description: Identifica o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo).
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fbc2fd2f6c93cac583fc1ec28375d8538d35b447
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135755"
---
# <a name="auditactivityinitiator-resource-type"></a>Tipo de recurso auditActivityInitiator

Namespace: microsoft.graph

Identidade do objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado um aplicativo).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aplicativo|[appIdentity](appidentity.md)|Se o recurso que inicia a atividade for um aplicativo, essa propriedade indicará todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalId, Name.|
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

