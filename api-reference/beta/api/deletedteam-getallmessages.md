---
title: 'deletedTeam: getAllMessages'
description: Recuperar todas as mensagens entre os todos os canais em uma equipe excluída.
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ddb94c35b00a88041004d01567d572d157af84a9
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578113"
---
# <a name="deletedteam-getallmessages"></a>deletedTeam: getAllMessages
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar todas as [mensagens](../resources/chatmessage.md) em todos os [canais](../resources/channel.md) em uma [equipe excluída](../resources/deletedteam.md), incluindo conversas de texto, áudio e vídeo.

Para saber mais sobre o uso das APIs de exportação do Microsoft Teams para exportar conteúdo, consulte [Exportar conteúdo com as APIs de Exportação do Microsoft Teams](/microsoftteams/export-teams-content).

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Sem suporte.|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ChannelMessage.Read.All|

> [!NOTE]
> Antes de chamar essa API com permissões de aplicativo, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Você pode usar o `model` parâmetro de consulta, que suporta os valores `A` e `B`, com base no preferido [modelo de licenciamento e pagamento](/graph/teams-licenses), como mostrado nos seguintes exemplos.  

```http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=A
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=B
```

Se o `model` parâmetro não for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

Este método dá suporte ao parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta e o parâmetro de consulta [$filter](/graph/query-parameters#filter-parameter) com intervalo de consultas **Data/Hora** em **lastModifiedDateTime**. Outros [Parâmetros de consulta do Protocolo Open Data](/graph/query-parameters) não têm suporte no momento.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedida, esta função devolve um `200 OK`código de resposta e uma coleção de objetos de [chatMessage](../resources/chatmessage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "deletedteamthis_getallmessages"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990417393",
            "replyToId": null,
            "etag": "1616990417393",
            "messageType": "message",
            "createdDateTime": "2021-03-29T04:00:17.393Z",
            "lastModifiedDateTime": "2021-03-29T04:00:17.393Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Ad5d2708d408c41d98424c1c354c19db3%40thread.tacv2/1616990417393?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990417393&parentMessageId=1616990417393",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test message"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:d5d2708d408c41d98424c1c354c19db3@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

