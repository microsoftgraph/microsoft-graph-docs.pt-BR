---
title: Atualizar membro no Team
description: Atualizar a função de membro em uma equipe.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f2da331041c01aa5fbfb3201f3fb656a7ee1fa24
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387851"
---
# <a name="update-member-in-team"></a>Atualizar membro no Team

Namespace: microsoft.graph

Atualizar a função de um [conversationMember](../resources/conversationmember.md) em uma [equipe](../resources/team.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)|TeamMember. ReadWrite. All. |
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|TeamMember. ReadWrite. All. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|funções|coleção de cadeias de caracteres|A função para o usuário. Deve ser `owner` ou vazio. Os usuários convidados são automaticamente carimbados com `guest` a função e esse valor não pode ser atualizado. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

A seguir está uma solicitação para aplicar a `owner` função a um membro existente de uma equipe.

<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a>Confira também

- [Atualizar membro no canal](channel-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of team member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
