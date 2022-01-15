---
title: Tipo de recurso microsoftAccountUserConversationMember
description: Representa um usuário de conta pessoal da Microsoft em um chat.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6d68d9bf9aa32bbb0965f5a892cd923627266c8e
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056360"
---
# <a name="microsoftaccountuserconversationmember-resource-type"></a>Tipo de recurso microsoftAccountUserConversationMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário de conta pessoal da Microsoft em um chat.


Herda de [conversationMember](../resources/conversationmember.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do usuário. Herdado [de conversationMember](../resources/conversationmember.md).|
|id|Cadeia de caracteres|ID de associação que representa esse recurso. Herdado da [entidade](../resources/entity.md).|
|funções|Coleção de cadeias de caracteres|Funções especiais para esse usuário. Herdado [de conversationMember](../resources/conversationmember.md).|
|userId|Cadeia de caracteres|ID do usuário.|
|visibleHistoryStartDateTime|DateTimeOffset|O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa. Herdado [de conversationMember](../resources/conversationmember.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAccountUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAccountUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String"
}
```

