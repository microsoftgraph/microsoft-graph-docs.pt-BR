---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ca1b7b0a2ae4021dc2def637e0326044ab8749e
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331344"
---
# <a name="groupmembers-complex-type"></a>tipo complexo groupMembers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). O `@odata.type` valor "`#microsoft.graph.groupMembers`" indica que esse tipo identifica uma coleção de usuários no locatário que será permitido como solicitante, Aprovador ou revisor, que são os membros de um grupo específico.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |Cadeia de caracteres | A ID do grupo no Azure AD. |
| descrição |String | O nome do grupo no Azure AD. Somente leitura. |
| IsBackup | Booliano | Para o **groupMembers** em um estágio de aprovação, essa propriedade indica que os membros do grupo são aprovadores de fallback de backup. |

## <a name="json-representation"></a>Representação JSON


Veja a seguir uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
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
