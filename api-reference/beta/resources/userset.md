---
title: Tipo complexo userSet
description: O tipo base abstrato para tipos usados nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a36ca6012c86486ae2eba0a2f73cce401d5609d9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136127"
---
# <a name="userset-complex-type"></a>Tipo complexo userSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) O tipo de base abstrata para [o singleUser](singleuser.md),[groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)e [externalSponsors](externalsponsors.md) tipos.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Para um usuário em um estágio de aprovação, essa propriedade indica se o usuário é um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de userSet.  Observe que um userSet é uma classe base abstrata e, portanto, não seria enviado ou recebido.  Em vez disso, um dos `@odata.type` " `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` ", " `#microsoft.graph.connectedOrganizationMembers` " `#microsoft.graph.requestorManager` ", " " ou " `#microsoft.graph.internalSponsors` seria `#microsoft.graph.externalSponsors` usado.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet"
}-->

```json
{
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


