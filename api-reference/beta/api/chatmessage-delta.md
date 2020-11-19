---
title: 'chatMessages: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 7ed834091507962a76e1e5384791d9ebcfb80666
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255474"
---
# <a name="chatmessages-delta"></a>chatMessages: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [ canal](../resources/channel.md) de uma [ equipe ](../resources/team.md). Usando a consulta delta, você pode obter mensagens novas ou atualizadas em um canal.

> **Observação:** A Delta só retornará mensagens dentro dos últimos oito meses. Você pode usar [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) para recuperar mensagens mais antigas.

A consulta Delta suporta tanto a sincronização total que recupera todas as mensagens no canal especificado e a sincronização incremental que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização. Tipicamente, você faria uma sincronização inicial completa, e então obteria mudanças incrementais modo de exibição Calendário periodicamente.

Para obter as respostas de uma mensagem, use a operação [list message replies](channel-get-messagereply.md) ou [get message reply](channel-list-messagereplies.md).

Uma solicitação GET com a função delta traz como resultado uma destas opções:

- Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou
- A `deltaLink` (que contém uma URL com uma chamada de função **delta** e `deltaToken`).

As fichas de estado são completamente opacas para o cliente. Para proceder com uma rodada de rastreamento de mudanças, basta copiar e aplicar o `nextLink` ou o `deltaLink`. URL retornado da última solicitação GET para a próxima chamada de função delta para o mesmo modo de exibição Calendário. Um `deltaLink` retornado em uma resposta significa que a rodada atual de rastreamento de mudanças está completa. Você pode salvar e usar o `deltaLink`. URL quando você começar a próxima rodada.

Para mais informações, confira a documentação [delta query](/graph/delta-query-overview).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).

|Tipo de permissão                        |Permissões (da com menos para a com mais privilégios)  |
|---------------------------------------|---------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) |Não suportado                                |
|Aplicativo                            | ChannelMessage.Read.Group*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All |

> **Observação**: Permissões marcadas com * usar [consentimento específico de recursos]( https://aka.ms/teams-rsc).

> [!NOTE]
> Antes de chamar esta API com permissões de aplicação, você deve solicitar acesso. Para detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O rastreamento de alterações nas mensagens do canal incorre em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), deverá especificá-lo na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados na parte do token do URL `nextLink` ou `deltaLink` fornecido na réplica.

Você só precisa especificar quaisquer parâmetros de consulta uma vez com antecedência.

Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `$deltatoken` | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado no `deltaLink` URL da chamada de função **delta** anterior, indicando a conclusão dessa rodada de acompanhamento de alterações. Salve e aplique o URL `deltaLink` inteiro, incluindo este token, na primeira solicitação da próxima rodada de acompanhamento de alterações para essa coleção.|
| `$skiptoken` | cadeia de caracteres | Um [ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas. |

### <a name="optional-odata-query-parameters"></a>Parâmetros de consulta OData opcionais

Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatíveis com esta API:
- `$top`, representa o número máximo de mensagens a serem buscadas em uma chamada. O limite superior é **50**.
- `$skip`, representa quantas mensagens ignorar no início da lista.
- `$filter` permite retornar mensagens que atendam a determinados critérios. A única propriedade que oferece suporte à filtragem é `lastModifiedDateTime`, e apenas o operador **gt** é compatível. Por exemplo, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` irá buscar todas as mensagens criadas ou alteradas após a data e hora especificada.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho        | Valor                     |
|---------------|---------------------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Corpo da Solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta. A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.

## <a name="examples"></a>Exemplos

### <a name="example-1-initial-synchronization"></a>Exemplo 1: Sincronização inicial

O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens em determinado canal. Há cinco mensagens no canal.

- Etapa 1: [amostra de solicitação inicial](#initial-request) e [resposta](#initial-request-response).
- Etapa 2:[ segundo exemplo de solicitação](#second-request) e [resposta](#second-request-response)
- Etapa 3:[ terceiro exemplo de solicitação](#third-request) e [resposta final](#third-request-response).

Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.

Confira também o que você vai fazer na [próxima fase](#example-2-retrieving-additional-changes).

#### <a name="initial-request"></a>Solicitação inicial

Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto, a solicitação de sincronização inicial não inclui nenhum token de estado. Esta rodada retornará todos os eventos no modo de exibição Calendário.

A solicitação especifica o cabeçalho opcional da solicitação, odata.top, retornando 2 eventos por vez.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a>Resposta à solicitação inicial

A resposta inclui duas mensagens e um `@odata.nextLink` cabeçalho de resposta com um `skipToken`. O URL `nextLink` indica que há mais mensagens no canal a serem obtidas.

>**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T07:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T07:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T08:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T08:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="second-request"></a>Segunda solicitação

A segunda solicitação especifica o `nextLink` URL retornado da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros principais da solicitação inicial, pois o `skipToken` no `nextLink` URL os codifica e inclui.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a>Resposta da segunda solicitação

A segunda resposta retorna as próximas 2 mensagens e um `@odata.nextLink` cabeçalho de resposta com um `skipToken`, indica que há mais mensagens no canal a serem obtidas.

>**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:50:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:50:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="third-request"></a>Terceira solicitação

A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a>Terceira solicitação de réplica

A terceira réplica retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas. Salve e use o `deltaLink` URL para consultar quaisquer novas mensagens a partir deste ponto na próxima rodada.

>**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a>Exemplo 2: Recuperando alterações adicionais

Usando o `deltaLink` da última solicitação na última rodada, você será capaz de obter apenas as mensagens que foram alteradas (ao serem adicionadas ou atualizadas) naquele canal desde então. Sua solicitação será semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo da página na réplica:

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Channel messages: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    ]
}
-->


