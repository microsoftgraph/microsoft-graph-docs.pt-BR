---
title: Listar membros de um canal
description: Liste os membros de um canal.
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1d0dd4bc81639d7ae4048635672b528c02146ee8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008822"
---
# <a name="list-members-of-a-channel"></a>Listar membros de um canal

Namespace: microsoft.graph

Recupere a lista [conversationMembers](../resources/conversationmember.md) de um [canal](../resources/channel.md).

> [!NOTE]
> As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas. O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.
>
> Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegada (conta corporativa ou de estudante)|ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ChannelMember.Read.All, ChannelMember.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored"} -->

```http
GET /teams/{team-id}/channels/{channel-id}/members
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel-list_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/2ab9c796-2902-45f8-b712-7c5a63cf41c4/channels/19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-list-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-list-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-list-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-list-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/channel-list-member-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
"@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('2ab9c796-2902-45f8-b712-7c5a63cf41c4')/channels('19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype')/members",
"@odata.count": 2,
"value": [
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ=",
        "roles": [],
        "displayName": "Jane Doe",
        "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
        "email": "jdoe@teamsip.onmicrosoft.com"
    },
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNiMzI0NmY0NC1jMDkxLTQ2MjctOTZjNi0yNWIxOGZhMmM5MTA=",
        "roles": [
            "owner"
        ],
        "displayName": "Ace John",
        "userId": "b3246f44-c091-4627-96c6-25b18fa2c910",
        "email": "ajohn@teamsip.onmicrosoft.com"
    }
]
}

```

## <a name="see-also"></a>Confira também

- [Listar membros de equipe](team-list-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
