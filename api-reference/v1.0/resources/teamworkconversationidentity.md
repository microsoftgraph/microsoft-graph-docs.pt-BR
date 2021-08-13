---
title: Tipo de recurso teamworkConversationIdentity
description: Representa uma conversa em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe6315b6546d603c203fad878c291f61e1f8394fc56acba4cfdf788ee86a2856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249108"
---
# <a name="teamworkconversationidentity-resource-type"></a>Tipo de recurso teamworkConversationIdentity

Namespace: microsoft.graph

Representa uma **conversa** (chat, equipe ou canal) no Microsoft Teams.

Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conversationIdentityType|teamworkConversationIdentityType|Tipo de conversa. Os valores possíveis são: `team`, `channel`, `chat`, e `unknownFutureValue`.|
|displayName|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). Nome de exibição da conversa. Opcional.|
|id|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). ID da conversa.|

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

