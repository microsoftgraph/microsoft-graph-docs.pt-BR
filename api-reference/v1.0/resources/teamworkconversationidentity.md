---
title: Tipo de recurso teamworkConversationIdentity
description: Representa uma conversa em Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a463f37152b6d2108ac6ca04d9971cb908d6ba4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055826"
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

