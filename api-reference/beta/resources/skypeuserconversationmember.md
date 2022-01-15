---
title: Tipo de recurso skypeUserConversationMember
description: Representa um Skype usuário em um chat
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c31f0af2f7e61783e540e0fa1a714fd846deed8d
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056349"
---
# <a name="skypeuserconversationmember-resource-type"></a>Tipo de recurso skypeUserConversationMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um Skype (consumidor) em um chat. 

Para obter informações sobre Teams e Skype for Business interoperabilidade, consulte [Understand Microsoft Teams and Skype for Business coexistence and interoperability](/microsoftteams/teams-and-skypeforbusiness-coexistence-and-interoperability).

Herda de [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do usuário. Herdado [de conversationMember](../resources/conversationmember.md).|
|id|Cadeia de caracteres|ID de associação que representa esse recurso. Herdado da [entidade](../resources/entity.md).|
|funções|Coleção de cadeias de caracteres|Funções especiais para esse usuário. Herdado [de conversationMember](../resources/conversationmember.md).|
|skypeId|Cadeia de caracteres|Skype ID do usuário.|
|visibleHistoryStartDateTime|DateTimeOffset|O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa. Herdado [de conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "skypeId": "String"
}
```

