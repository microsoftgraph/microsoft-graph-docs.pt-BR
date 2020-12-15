---
title: 'conversationMember: adicionar'
description: Adicionar membros em massa à equipe.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ffc3d9d36c0f4d22653a961ebe5af4769f286d7d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658324"
---
# <a name="conversationmember-add"></a>conversationMember: adicionar

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione vários membros em uma única solicitação a uma [equipe](../resources/team.md). A resposta fornece detalhes sobre quais associações podem e não podem ser criadas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios) | 
|:--------------------|:--------------------------|
| Delegado (conta corporativa ou de estudante) | TeamMember.ReadWrite.All  |
| Delegado (conta pessoal da Microsoft) | Sem suporte |
| Aplicativo | TeamMember.ReadWrite.All   |


## <a name="http-request"></a>Solicitação HTTP

Esta é uma ação vinculada para adicionar vários elementos a uma coleção **chatMember** em uma única solicitação.
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça a representação JSON da lista de `conversationMember` derivados que precisam ser adicionados à equipe.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|values|coleção [conversationMember](../resources/conversationmember.md)|Lista de membros da conversa que devem ser adicionados.|


## <a name="response"></a>Resposta

Se bem-sucedida, esta ação retorna um código de resposta `200 OK`e uma coleção de derivados de [actionResultPart](../resources/actionresultpart.md) no corpo da resposta.

Esta API retorna uma resposta `200` indicando que todos os membros fornecidos foram adicionados à equipe ou uma resposta `207` indicando que apenas alguns dos membros fornecidos foram adicionados à equipe. O chamador deve inspecionar a carga útil de resposta para determinar quais adições de membro falharam. O corpo da resposta é uma coleção de derivados do recurso [actionResultPart](../resources/actionresultpart.md).

## <a name="examples"></a>Exemplos

### <a name="example-1-add-members-in-bulk-to-a-team"></a>Exemplo 1: adicionar membros em massa a uma equipe

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe.
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```

#### <a name="response"></a>Resposta

Esta é a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.aadUserConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": null
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a>Exemplo 2: adicionar membros em massa e encontrar falha parcial

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para adicionar vários membros a uma equipe que resulta em uma falha parcial.

<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team_partial_failure"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```

#### <a name="response"></a>Resposta

Esta é a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 207 MULTI-STATUS
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.addConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": {
                "code": "NotFound",
                "message": ""
            }
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```


## <a name="see-also"></a>Confira também

- [Adicionar membro à equipe](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add members to team in bulk",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
