---
title: 'chatMessages: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: e5f297dc236899f0fbd362c7ef369897b7bc7786
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719854"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="93183-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="93183-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93183-105">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="93183-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="93183-106">Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.</span><span class="sxs-lookup"><span data-stu-id="93183-106">By using delta query, you can get new, updated, or deleted events in a calendar view.</span></span>

<span data-ttu-id="93183-107">A consulta Delta é compatível tanto com sincronização completa que recupera todos as mensagens num canal especificado quanto com a sincronização incremental que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="93183-107">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization.</span></span> <span data-ttu-id="93183-108">Normalmente, você faria uma sincronização total inicial e, logo depois, obteria periodicamente alterações incrementais para esse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="93183-108">Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="93183-109">Para obter as respostas de uma mensagem, utilize use a operação [listar respostas da mensagem](channel-get-messagereply.md) ou a operação [obter resposta da mensagem](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="93183-109">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span>

<span data-ttu-id="93183-110">Uma solicitação GET com a função delta traz como resultado uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="93183-110">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="93183-111">Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou</span><span class="sxs-lookup"><span data-stu-id="93183-111">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="93183-112">Uma `deltaLink` (que contém uma URL com uma chamada de função **delta** e `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="93183-112">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="93183-113">Os tokens de estado são completamente opacos para o cliente.</span><span class="sxs-lookup"><span data-stu-id="93183-113">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="93183-114">Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função delta do mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="93183-114">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="93183-115">Um `deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída.</span><span class="sxs-lookup"><span data-stu-id="93183-115">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="93183-116">Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="93183-116">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="93183-117">Para obter mais informações, consulte a documentação da [consulta Delta](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="93183-117">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="93183-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="93183-118">Permissions</span></span>

<span data-ttu-id="93183-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93183-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="93183-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93183-121">Permission Type</span></span>                        |<span data-ttu-id="93183-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93183-122">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="93183-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93183-123">Delegated (work or school account)</span></span>     |<span data-ttu-id="93183-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93183-124">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="93183-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93183-125">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="93183-126">Não suportado</span><span class="sxs-lookup"><span data-stu-id="93183-126">Not Supported</span></span>                                |
|<span data-ttu-id="93183-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93183-127">Application</span></span>                            |<span data-ttu-id="93183-128">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93183-128">Group.Read.All, Group.ReadWrite.All</span></span>          |

## <a name="http-request"></a><span data-ttu-id="93183-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93183-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="93183-130">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="93183-130">Query parameters</span></span>

<span data-ttu-id="93183-131">O controle de alterações nas mensagens de canal gera uma série de uma ou mais chamadas de função **delta**.</span><span class="sxs-lookup"><span data-stu-id="93183-131">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="93183-132">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="93183-132">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="93183-133">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="93183-133">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="93183-134">Você só precisa especificar uma vez antecipadamente os parâmetros de consulta desejados.</span><span class="sxs-lookup"><span data-stu-id="93183-134">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="93183-135">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="93183-135">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="93183-136">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="93183-136">Query parameter</span></span>      | <span data-ttu-id="93183-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="93183-137">Type</span></span>   |<span data-ttu-id="93183-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="93183-138">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="93183-139">string</span><span class="sxs-lookup"><span data-stu-id="93183-139">string</span></span> | <span data-ttu-id="93183-140">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior, indicando a conclusão daquela série de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="93183-140">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire  URL including this token in the first request of the next round of change tracking for that collection.</span></span> <span data-ttu-id="93183-141">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="93183-141">A state token returned in the  URL of the previous delta function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="93183-142">string</span><span class="sxs-lookup"><span data-stu-id="93183-142">string</span></span> | <span data-ttu-id="93183-143">Um[ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas.</span><span class="sxs-lookup"><span data-stu-id="93183-143">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="93183-144">Parâmetros de consulta OData opcionais</span><span class="sxs-lookup"><span data-stu-id="93183-144">Optional OData query parameters</span></span>

<span data-ttu-id="93183-145">Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatível com esta API:</span><span class="sxs-lookup"><span data-stu-id="93183-145">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="93183-146">`$top`representa o número máximo de mensagens a buscar em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="93183-146">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="93183-147">O limite máximo é **50**.</span><span class="sxs-lookup"><span data-stu-id="93183-147">The upper limit is **50**.</span></span>
- <span data-ttu-id="93183-148">`$skip`representa quantas mensagens devem ser ignoradas no início da lista.</span><span class="sxs-lookup"><span data-stu-id="93183-148">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="93183-149">`$filter` permite retornar mensagens que atendem a certos critérios.</span><span class="sxs-lookup"><span data-stu-id="93183-149">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="93183-150">A única propriedade que permite a filtragem é `lastModifiedDateTime`e somente os operadores **gt** e **ge** são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="93183-150">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** and **ge** operators are supported.</span></span> <span data-ttu-id="93183-151">Por exemplo, o`../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` vai buscar todas as mensagens criadas ou alteradas após o período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="93183-151">For example, `../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93183-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-152">Request headers</span></span>
| <span data-ttu-id="93183-153">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93183-153">Header</span></span>        | <span data-ttu-id="93183-154">Valor</span><span class="sxs-lookup"><span data-stu-id="93183-154">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="93183-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="93183-155">Authorization</span></span> | <span data-ttu-id="93183-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93183-p110">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93183-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93183-158">Content-Type</span></span>  | <span data-ttu-id="93183-159">application/json</span><span class="sxs-lookup"><span data-stu-id="93183-159">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="93183-160">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-160">Request body</span></span>

<span data-ttu-id="93183-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93183-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93183-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="93183-162">Response</span></span>

<span data-ttu-id="93183-163">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](https://docs.microsoft.com/pt-BR/graph/api/resources/chatmessage?view=graph-rest-beta) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93183-163">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](https://docs.microsoft.com/en-us/graph/api/resources/chatmessage?view=graph-rest-beta) objects in the response body.</span></span> <span data-ttu-id="93183-164">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="93183-164">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="93183-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93183-165">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="93183-166">Exemplo 1: sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="93183-166">Example 1: Initial synchronization</span></span>

<span data-ttu-id="93183-167">O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens num dado canal.</span><span class="sxs-lookup"><span data-stu-id="93183-167">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="93183-168">Há cinco mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="93183-168">There are five messages in the channel.</span></span>

- <span data-ttu-id="93183-169">Etapa 1:[ exemplo inicial de solicitação](#initial-request) e [resposta](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="93183-169">[Step 1: sample initial request](#initial-request) and [response](#initial-request-response)</span></span>
- <span data-ttu-id="93183-170">Etapa 2:[ segundo exemplo de solicitação](#second-request) e [resposta](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="93183-170">[Step 2: sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="93183-171">Etapa 3:[ terceiro exemplo de solicitação](#third-request) e [resposta final](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="93183-171">[Step 3: sample third request](#third-request) and [final response](#third-request-response)</span></span>

<span data-ttu-id="93183-p113">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="93183-p113">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="93183-174">Confira também o que você vai fazer na [próxima fase](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="93183-174">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="93183-175">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="93183-175">Initial request</span></span>

<span data-ttu-id="93183-176">Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto a solicitação de sincronização inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="93183-176">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="93183-177">Essa rodada mostrará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="93183-177">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="93183-178">A solicitação especifica o cabeçalho de solicitação opcional, odata.top, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="93183-178">The optional request header, odata.maxpagesize, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93183-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="93183-179">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93183-180">C#</span><span class="sxs-lookup"><span data-stu-id="93183-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93183-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93183-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93183-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93183-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="93183-183">Resposta inicial da solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-183">Initial request and response</span></span>

<span data-ttu-id="93183-184">A resposta inclui duas mensagens e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="93183-184">The response includes two events and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="93183-185">A URL `nextLink` indica que há mais mensagens na pasta a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="93183-185">The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

><span data-ttu-id="93183-186">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="93183-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93183-187">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93183-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
            "from" : {
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

#### <a name="second-request"></a><span data-ttu-id="93183-188">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-188">Second request</span></span>

<span data-ttu-id="93183-189">A segunda solicitação especifica a URL `nextLink` retornada na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="93183-189">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="93183-190">Observe que não é mais necessário especificar os mesmos parâmetros principais definidos na solicitação inicial, pois o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="93183-190">Notice that it no longer has to specify the same startDateTime and endDateTime parameters as in the initial request, as the  in the  URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93183-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="93183-191">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93183-192">C#</span><span class="sxs-lookup"><span data-stu-id="93183-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93183-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93183-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93183-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93183-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="93183-195">Resposta da segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-195">Second request response</span></span>

<span data-ttu-id="93183-196">A segunda resposta retorna as 2 próximas mensagens e um `@odata.nextLink` cabeçalho de resposta com um`skipToken`, indicando que há mais mensagens para se obter no canal.</span><span class="sxs-lookup"><span data-stu-id="93183-196">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="93183-197">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="93183-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93183-198">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93183-198">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
            "from" : {
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

#### <a name="third-request"></a><span data-ttu-id="93183-199">Terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-199">Third sync request</span></span>

<span data-ttu-id="93183-200">A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="93183-200">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93183-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="93183-201">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93183-202">C#</span><span class="sxs-lookup"><span data-stu-id="93183-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93183-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93183-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93183-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93183-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="93183-205">Resposta da terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-205">Third request response</span></span>

<span data-ttu-id="93183-206">A terceira resposta retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas.</span><span class="sxs-lookup"><span data-stu-id="93183-206">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="93183-207">Salvar e usar a URL `deltaLink` para consultar novas mensagens a partir desse ponto na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="93183-207">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="93183-208">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="93183-208">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93183-209">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93183-209">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="93183-210">Exemplo 2: recuperar alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="93183-210">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="93183-211">Usando o `deltaLink` da última solicitação na última fase, você poderá obter somente as mensagens que sofreram alteração (por terem sido adicionadas, excluídas ou atualizadas) nesse canal desde então.</span><span class="sxs-lookup"><span data-stu-id="93183-211">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then.</span></span> <span data-ttu-id="93183-212">Supondo que você prefira manter o mesmo tamanho máximo de página na resposta, sua solicitação terá um formato semelhante a este :</span><span class="sxs-lookup"><span data-stu-id="93183-212">Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="93183-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93183-213">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93183-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="93183-214">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93183-215">C#</span><span class="sxs-lookup"><span data-stu-id="93183-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93183-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93183-216">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93183-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93183-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93183-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="93183-218">Response</span></span>

><span data-ttu-id="93183-p122">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93183-p122">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
