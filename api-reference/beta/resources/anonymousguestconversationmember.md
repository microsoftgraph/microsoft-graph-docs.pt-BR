---
title: Tipo de recurso anonymousGuestConversationMember
description: Representa um convidado anônimo em um chat.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f439daa2e5146b37b94862e2dce87a2efb603f02
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056350"
---
# <a name="anonymousguestconversationmember-resource-type"></a>Tipo de recurso anonymousGuestConversationMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um convidado anônimo em um chat. 

Os usuários anônimos não têm uma identidade Microsoft Teams e podem participar de reuniões usando links de junção de reunião. Para obter mais detalhes, consulte [Usuários anônimos](/microsoftteams/non-standard-users#anonymous-users).


Herda de [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|anonymousGuestId|Cadeia de caracteres|ID exclusiva que representa o usuário. **Observação:** Essa ID pode mudar se o usuário sair e voltar à reunião ou ingressar em um dispositivo diferente.|
|displayName|Cadeia de caracteres|Nome fornecido pelo usuário ao ingressar na reunião. Herdado [de conversationMember](../resources/conversationmember.md).|
|id|String|ID de associação que representa esse recurso. Herdado da [entidade](../resources/entity.md).|
|funções|Coleção de cadeias de caracteres|Funções especiais para esse usuário. Herdado [de conversationMember](../resources/conversationmember.md).|
|visibleHistoryStartDateTime|DateTimeOffset|O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa. Herdado [de conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.anonymousGuestConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.anonymousGuestConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "anonymousGuestId": "String"
}
```

