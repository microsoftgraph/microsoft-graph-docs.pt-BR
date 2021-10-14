---
title: Tipo complexo userSet
description: O tipo de base abstrata para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bd16a117b7b1bd93db1977ffb50ba501b4e801ed
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289529"
---
# <a name="userset-complex-type"></a>Tipo complexo userSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) É um tipo de base abstrato herdado pelos seguintes tipos de recurso:
+ [singleUser](singleuser.md)
+ [groupMembers](groupmembers.md)
+ [connectedOrganizationMembers](connectedorganizationmembers.md)
+ [requestorManager](requestormanager.md)
+ [internalSponsors](internalsponsors.md)
+ [externalSponsors](externalsponsors.md)

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Para um usuário em um estágio de aprovação, essa propriedade indica se o usuário é um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de userSet. Um [userSet](userset.md) é uma classe base abstrata e, portanto, não seria enviado ou recebido.  Em vez disso, um dos seguintes `@odata.type` valores que representam os tipos herdados seria usado:
+ `#microsoft.graph.singleUser`
+ `#microsoft.graph.groupMembers`
+ `#microsoft.graph.connectedOrganizationMembers`
+ `#microsoft.graph.requestorManager`
+ `#microsoft.graph.internalSponsors`
+ `#microsoft.graph.externalSponsors`

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.userSet",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


