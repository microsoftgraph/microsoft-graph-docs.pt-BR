---
title: 'chatMessages: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: b02032e06929a20f9835bed9249b68b2cada2b8e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000655"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="c75aa-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="c75aa-104">chatMessages: delta</span></span>

<span data-ttu-id="c75aa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c75aa-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c75aa-p102">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md). Usando a consulta delta, você pode obter mensagens novas ou atualizadas em um canal.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p102">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md). By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="c75aa-p103">**Observação:** Delta retornará mensagens apenas nos últimos oito meses. Você pode usar [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) para recuperar mensagens mais antigas.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p103">**Note:** Delta will only return messages within the last eight months. You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="c75aa-p104">A consulta delta oferece suporte à sincronização completa, que recupera todas as mensagens no canal especificado, e à sincronização incremental, que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização. Normalmente, você faria uma sincronização completa inicial e, em seguida, obteria mudanças incrementais nessa visualização do calendário periodicamente.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p104">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization. Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="c75aa-112">Para obter as respostas para uma mensagem, use a operação [listar respostas de mensagens](channel-get-messagereply.md) ou [obter resposta de mensagem](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="c75aa-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="c75aa-113">Uma solicitação GET com a função delta traz como resultado uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="c75aa-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="c75aa-114">Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou</span><span class="sxs-lookup"><span data-stu-id="c75aa-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="c75aa-115">Um `deltaLink` (que contém um URL com uma chamada de função **delta** e `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="c75aa-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="c75aa-p105">Os tokens de estado são completamente opacos para o cliente. Para prosseguir com uma rodada de controle de alterações, simplesmente copie e aplique o URL `nextLink` ou `deltaLink` retornado da última solicitação GET para a próxima chamada de função delta para essa mesma visualização de calendário. Um `deltaLink` retornado em uma resposta significa que a rodada atual de controle de alterações foi concluída. Você pode salvar e usar o `deltaLink` URL ao iniciar a próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="c75aa-120">Para obter mais informações, consulte a documentação da [consulta delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="c75aa-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c75aa-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="c75aa-121">Permissions</span></span>

<span data-ttu-id="c75aa-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c75aa-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="c75aa-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c75aa-124">Permission Type</span></span>                        |<span data-ttu-id="c75aa-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c75aa-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="c75aa-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c75aa-126">Delegated (work or school account)</span></span>| <span data-ttu-id="c75aa-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c75aa-127">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="c75aa-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c75aa-128">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c75aa-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c75aa-129">Not supported.</span></span>|
|<span data-ttu-id="c75aa-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c75aa-130">Application</span></span>| <span data-ttu-id="c75aa-131">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c75aa-131">Not supported.</span></span> |

> <span data-ttu-id="c75aa-132">**Observação** : As permissões marcadas com \* usam [ consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="c75aa-132">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="c75aa-p107">Antes de chamar esta API com permissões de aplicativo, você deve solicitar acesso. Para obter detalhes, consulte [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c75aa-p107">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c75aa-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c75aa-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c75aa-136">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="c75aa-136">Query parameters</span></span>

<span data-ttu-id="c75aa-p108">O rastreamento de alterações nas mensagens do canal incorre em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), deverá especificá-lo na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados na parte do token do URL `nextLink` ou `deltaLink` fornecido na resposta.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p108">Tracking changes in channel messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="c75aa-140">Você só precisa especificar quaisquer parâmetros de consulta uma vez com antecedência.</span><span class="sxs-lookup"><span data-stu-id="c75aa-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="c75aa-141">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="c75aa-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="c75aa-142">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="c75aa-142">Query parameter</span></span>      | <span data-ttu-id="c75aa-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="c75aa-143">Type</span></span>   |<span data-ttu-id="c75aa-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="c75aa-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="c75aa-145">string</span><span class="sxs-lookup"><span data-stu-id="c75aa-145">string</span></span> | <span data-ttu-id="c75aa-p109">Um [token de estado](/graph/delta-query-overview) retornado no `deltaLink` URL da chamada de função **delta** anterior, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique o URL `deltaLink` inteiro, incluindo este token, na primeira solicitação da próxima rodada de controle de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p109">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="c75aa-148">string</span><span class="sxs-lookup"><span data-stu-id="c75aa-148">string</span></span> | <span data-ttu-id="c75aa-149">Um [ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas.</span><span class="sxs-lookup"><span data-stu-id="c75aa-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="c75aa-150">Parâmetros de consulta OData opcionais</span><span class="sxs-lookup"><span data-stu-id="c75aa-150">Optional OData query parameters</span></span>

<span data-ttu-id="c75aa-151">Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatíveis com esta API:</span><span class="sxs-lookup"><span data-stu-id="c75aa-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="c75aa-p110">`$top`, representa o número máximo de mensagens a serem buscadas em uma chamada. O limite superior é **50**.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p110">`$top`, represents maximum number of messages to fetch in a call. The upper limit is **50**.</span></span>
- <span data-ttu-id="c75aa-154">`$skip`, representa quantas mensagens ignorar no início da lista.</span><span class="sxs-lookup"><span data-stu-id="c75aa-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="c75aa-p111">`$filter` permite retornar mensagens que atendam a determinados critérios. A única propriedade que oferece suporte à filtragem é `lastModifiedDateTime`, e apenas o operador **gt** é compatível. Por exemplo, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` irá buscar todas as mensagens criadas ou alteradas após a data e hora especificada.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p111">`$filter` allows returning messages that meet a certain criteria. The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported. For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c75aa-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-158">Request headers</span></span>
| <span data-ttu-id="c75aa-159">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c75aa-159">Header</span></span>        | <span data-ttu-id="c75aa-160">Valor</span><span class="sxs-lookup"><span data-stu-id="c75aa-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="c75aa-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="c75aa-161">Authorization</span></span> | <span data-ttu-id="c75aa-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c75aa-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c75aa-164">Content-Type</span></span>  | <span data-ttu-id="c75aa-165">application/json</span><span class="sxs-lookup"><span data-stu-id="c75aa-165">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c75aa-166">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-166">Request Body</span></span>

<span data-ttu-id="c75aa-167">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c75aa-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c75aa-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75aa-168">Response</span></span>

<span data-ttu-id="c75aa-p113">Se for bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta. A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p113">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body. The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="c75aa-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c75aa-171">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="c75aa-172">Exemplo 1: Sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="c75aa-172">Example 1: Initial synchronization</span></span>

<span data-ttu-id="c75aa-p114">O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens em determinado canal. Existem cinco mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p114">The following example shows a series of three requests to synchronize the messages in the given channel. There are five messages in the channel.</span></span>

- <span data-ttu-id="c75aa-175">Etapa 1: [amostra de solicitação inicial](#initial-request) e [resposta](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="c75aa-175">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="c75aa-176">Etapa 2:[ segundo exemplo de solicitação](#second-request) e [resposta](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="c75aa-176">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="c75aa-177">Etapa 3:[ terceiro exemplo de solicitação](#third-request) e [resposta final](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="c75aa-177">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="c75aa-p115">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="c75aa-180">Confira também o que você vai fazer na [próxima fase](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="c75aa-180">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="c75aa-181">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="c75aa-181">Initial request</span></span>

<span data-ttu-id="c75aa-p116">Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto, a solicitação de sincronização inicial não inclui nenhum token de estado. Esta rodada retornará todos os eventos nessa visualização de calendário.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p116">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="c75aa-184">A solicitação especifica o cabeçalho opcional da solicitação, odata.top, retornando 2 eventos por vez.</span><span class="sxs-lookup"><span data-stu-id="c75aa-184">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>



# <a name="http"></a>[<span data-ttu-id="c75aa-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="c75aa-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="c75aa-186">C#</span><span class="sxs-lookup"><span data-stu-id="c75aa-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c75aa-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c75aa-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c75aa-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c75aa-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c75aa-189">Java</span><span class="sxs-lookup"><span data-stu-id="c75aa-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="initial-request-response"></a><span data-ttu-id="c75aa-190">Resposta à solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="c75aa-190">Initial request response</span></span>

<span data-ttu-id="c75aa-p117">A resposta inclui duas mensagens e um `@odata.nextLink` cabeçalho de resposta com um `skipToken`. O URL `nextLink` indica que há mais mensagens no canal a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p117">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="c75aa-p118">**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="c75aa-195">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-195">Second request</span></span>

<span data-ttu-id="c75aa-p119">A segunda solicitação especifica o `nextLink` URL retornado da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros principais da solicitação inicial, pois o `skipToken` no `nextLink` URL os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p119">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="c75aa-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="c75aa-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="c75aa-199">C#</span><span class="sxs-lookup"><span data-stu-id="c75aa-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c75aa-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c75aa-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c75aa-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c75aa-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c75aa-202">Java</span><span class="sxs-lookup"><span data-stu-id="c75aa-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="second-request-response"></a><span data-ttu-id="c75aa-203">Resposta da segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-203">Second request response</span></span>

<span data-ttu-id="c75aa-204">A segunda resposta retorna as próximas 2 mensagens e um `@odata.nextLink` cabeçalho de resposta com um `skipToken`, indica que há mais mensagens no canal a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="c75aa-204">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="c75aa-p120">**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="c75aa-207">Terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-207">Third request</span></span>

<span data-ttu-id="c75aa-208">A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c75aa-208">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>



# <a name="http"></a>[<span data-ttu-id="c75aa-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="c75aa-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="c75aa-210">C#</span><span class="sxs-lookup"><span data-stu-id="c75aa-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c75aa-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c75aa-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c75aa-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c75aa-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c75aa-213">Java</span><span class="sxs-lookup"><span data-stu-id="c75aa-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="third-request-response"></a><span data-ttu-id="c75aa-214">Terceira resposta ao pedido</span><span class="sxs-lookup"><span data-stu-id="c75aa-214">Third request response</span></span>

<span data-ttu-id="c75aa-p121">A terceira resposta retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas. Salve e use o `deltaLink` URL para consultar quaisquer novas mensagens a partir deste ponto na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p121">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read. Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="c75aa-p122">**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p122">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="c75aa-219">Exemplo 2: Recuperando mudanças adicionais</span><span class="sxs-lookup"><span data-stu-id="c75aa-219">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="c75aa-p123">Usando o `deltaLink` da última solicitação na última rodada, você será capaz de obter apenas as mensagens que foram alteradas (ao serem adicionadas ou atualizadas) naquele canal desde então. Sua solicitação será semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo da página na resposta:</span><span class="sxs-lookup"><span data-stu-id="c75aa-p123">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then. Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="c75aa-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c75aa-222">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="c75aa-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="c75aa-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="c75aa-224">C#</span><span class="sxs-lookup"><span data-stu-id="c75aa-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c75aa-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c75aa-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c75aa-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c75aa-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c75aa-227">Java</span><span class="sxs-lookup"><span data-stu-id="c75aa-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="c75aa-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75aa-228">Response</span></span>

><span data-ttu-id="c75aa-p124">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c75aa-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


