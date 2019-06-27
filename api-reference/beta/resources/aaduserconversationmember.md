---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário em uma conversa.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: fd326482869d9f72778edc9d4c55996f7aa59045
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236458"
---
# <a name="aaduserconversationmember-resource-type"></a>tipo de recurso aadUserConversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário do Azure Active Directory em um [bate-papo](chat.md). Esse tipo é herdado do [conversationMember](conversationmember.md).

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
|userId| cadeia de caracteres | O guid do usuário. |
|email| cadeia de caracteres  | O endereço de email do usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
