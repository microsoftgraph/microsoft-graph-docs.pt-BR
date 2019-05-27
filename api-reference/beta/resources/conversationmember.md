---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379266"
---
# <a name="conversationmember-resource-type"></a>tipo de recurso conversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em um [bate-papo](chat.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros do bate-papo](../api/conversationmember-list.md) | coleção [conversationmember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.|
|[Obter membro do bate-papo](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | Obter um único usuário no bate-papo.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusivo do usuário.|
|displayName| cadeia de caracteres | O nome de exibição do usuário. |
|funções| coleção de cadeias de caracteres | As funções desse usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a>Confira também

[aadUserConversationMember](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
