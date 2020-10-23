---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6057c8cf71ce0f8d71632267d3790c39b69b1eb1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735761"
---
# <a name="aaduserconversationmember-resource-type"></a>tipo de recurso aadUserConversationMember

Namespace: microsoft.graph

Representa um usuário do Azure Active Directory em uma [equipe](team.md).
Esse tipo é herdado do [conversationMember](conversationmember.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros](../api/conversationmember-list.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no chat ou canal.|
|[Obter membro](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Obter um único usuário no chat ou canal.|
|[Adicionar membro](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Adicionar um membro a um canal.|
|[Atualizar membro](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Atualizar um membro no canal.|
|[Excluir membro](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Excluir um membro do canal.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
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

