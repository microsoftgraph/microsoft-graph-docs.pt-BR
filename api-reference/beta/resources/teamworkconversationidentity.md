---
title: Tipo de recurso teamworkConversationIdentity
description: Representa uma conversa em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 84e936368b7cc4589b7611b15cf310f92b055e2a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211189"
---
# <a name="teamworkconversationidentity-resource-type"></a>Tipo de recurso teamworkConversationIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma **conversa** (chat, equipe ou canal) no Microsoft Teams.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conversationIdentityType|teamworkConversationIdentityType|Tipo de conversa. Os valores possíveis são: `team` `channel` , e `chat` .|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição da conversa. Opcional.|
|id|String|Herdado da [identidade](../resources/identity.md). ID da conversa.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

