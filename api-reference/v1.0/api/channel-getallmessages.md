---
title: 'channel: getAllMessages'
description: Recupere todas as mensagens entre os canais de uma equipe.
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
---

# <a name="channel-getallmessages"></a>channel: getAllMessages

Namespace: microsoft.graph

Recupere as [mensagens](../resources/chatmessage.md) em todos os [canais](../resources/channel.md) de uma [equipe](../resources/team.md), incluindo texto, áudio, e conversas de vídeo.

Para saber mais sobre como usar as APIs de exportação do Microsoft Teams para exportar conteúdo, consulte [Exportar conteúdo com as APIs de exportação do Microsoft Teams](/microsoftteams/export-teams-content).

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>Permissões

As seguintes permissões são obrigatórias para chamar esta API. Para saber mais, incluindo como escolher as permissões, consulte [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | ChannelMessage.Read.All |

> [!NOTE]
> Antes de chamar essa API com permissões de aplicativo, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
``` http
GET /teams/{team-id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Você pode usar o parâmetro de consulta `model`, que suporta os valores `A` e `B`, com base nos requisitos preferenciais de [modelo de licenciamento e pagamento](/graph/teams-licenses), como mostrado nos exemplos a seguir.  
Se nenhum `model` for especificado, [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

```http
GET /teams/{team-id}/channels/getAllMessages?model=A
GET /teams/{team-id}/channels/getAllMessages?model=B
```

Se nenhum `model` for especificado, [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado. 

Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.
Além disso, [$filter](/graph/query-parameters#filter-parameter) é suportado com **dateTime** intervalo de consulta em **lastModifiedDateTime**. Os outros [parâmetros de consulta OData](/graph/query-parameters) não têm suporte no momento.

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` de resposta e também retornará todas as mensagens em todos os canais públicos e privados.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_getallchannelmessages_1"
}-->
``` http
GET https://graph.microsoft.com/v1.0/teams/01fe12e0-e720-44fd-8854-28c66d1bee40/channels/getAllMessages?$filter=lastModifiedDateTime+gt+2019-11-01T00:00:00Z+and lastModifiedDateTime+lt+2021-11-01T00:00:00Z
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-getallchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-getallchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-getallchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-getallchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/channel-getallchannelmessages-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams('01fe12e0-e720-44fd-8854-28c66d1bee40')/channels/getallMessages?$skiptoken=U2tpcFZhbHVlPTAjUHJpdmF0ZUNoYW5uZWxJZD0xOTpmYWU5YTJmZjk1ZGE0ZTEwOWE1YTg3ZTM5Y2FkOGYyYkB0aHJlYWQudGFjdjIjVXNlcklkPTBkN2M2M2QzLTEzMDYtNGVlYy04ZjIxLTU4OGE3MGZiNmVmMSNNYWlsYm94Rm9sZGVyPU1haWxGb2xkZXJzL1RlYW1DaGF0&$filter=lastModifiedDateTime+gt+2019-11-01T00%3a00%3a00Z+and+lastModifiedDateTime+lt+2021-11-01T00%3a00%3a00Z",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1622071758431",
            "replyToId": "1622071642456",
            "etag": "1622071758431",
            "messageType": "message",
            "createdDateTime": "2021-05-26T23:29:18.431Z",
            "lastModifiedDateTime": "2021-05-26T23:29:18.431Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Afae9a2ff95da4e109a5a87e39cad8f2b%40thread.tacv2/1622071758431?groupId=01fe12e0-e720-44fd-8854-28c66d1bee40&tenantId=9854dc85-3fb3-4f8e-a055-9cdc5523024d&createdTime=1622071758431&parentMessageId=1622071642456",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>\n<div itemprop=\"copy-paste-block\">reply 9&nbsp;to new conv</div>\n</div>"
            },
            "channelIdentity": {
                "teamId": "01fe12e0-e720-44fd-8854-28c66d1bee40",
                "channelId": "19:fae9a2ff95da4e109a5a87e39cad8f2b@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1622071764529",
            "replyToId": "1622071642456",
            "etag": "1622071764529",
            "messageType": "message",
            "createdDateTime": "2021-05-26T23:29:24.529Z",
            "lastModifiedDateTime": "2021-05-26T23:29:24.529Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Afae9a2ff95da4e109a5a87e39cad8f2b%40thread.tacv2/1622071764529?groupId=01fe12e0-e720-44fd-8854-28c66d1bee40&tenantId=9854dc85-3fb3-4f8e-a055-9cdc5523024d&createdTime=1622071764529&parentMessageId=1622071642456",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>\n<div itemprop=\"copy-paste-block\">reply 10 to new conv</div>\n</div>"
            },
            "channelIdentity": {
                "teamId": "01fe12e0-e720-44fd-8854-28c66d1bee40",
                "channelId": "19:fae9a2ff95da4e109a5a87e39cad8f2b@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
