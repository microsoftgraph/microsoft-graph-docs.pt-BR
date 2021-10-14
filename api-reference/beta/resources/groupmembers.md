---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ce18ed739e1701e004c92f408d0276ef17f5d264
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289956"
---
# <a name="groupmembers-complex-type"></a>tipo complexo groupMembers

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) O valor indica que esse tipo identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou `@odata.type` revisor, que são membros de um `#microsoft.graph.groupMembers` grupo específico.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |String | A ID do grupo no Azure AD. |
| description |String | O nome do grupo no Azure AD. Somente leitura. |
| isBackup | Boolean | Para **groupMembers** em um estágio de aprovação, essa propriedade indica que os membros do grupo são um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON


A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


