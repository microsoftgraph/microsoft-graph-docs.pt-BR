---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d2df6b91ebcbc65f03ee39103768bdfad04df62f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027192"
---
# <a name="connectedorganizationmembers-complex-type"></a>tipo complexo connectedOrganizationMembers

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). O `@odata.type` valor `#microsoft.graph.connectedOrganizationMembers` indica que esse tipo identifica uma coleção de usuários, os que estão associados a uma [organização conectada](connectedorganization.md), que terá permissão para solicitar um pacote do Access.

## <a name="properties"></a>Propriedades

Este tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |String | A ID da organização conectada no gerenciamento de qualificação. |
| description |String | O nome da organização conectada. Somente leitura. |
| IsBackup | Booliano | Não usado no momento. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
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
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


