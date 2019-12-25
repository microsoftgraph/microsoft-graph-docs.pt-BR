---
title: 'chatMessages: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a843044238a954d0c03136860c4f5289497797b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868118"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="dea8c-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="dea8c-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea8c-105">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dea8c-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="dea8c-106">Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.</span><span class="sxs-lookup"><span data-stu-id="dea8c-106">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="dea8c-107">**Observação:** Delta retornará apenas as mensagens dos últimos oito meses.</span><span class="sxs-lookup"><span data-stu-id="dea8c-107">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="dea8c-108">Você pode usar [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) para recuperar mensagens mais antigas.</span><span class="sxs-lookup"><span data-stu-id="dea8c-108">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="dea8c-109">A consulta Delta é compatível tanto com sincronização completa que recupera todos as mensagens num canal especificado quanto com a sincronização incremental que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="dea8c-109">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="dea8c-110">Normalmente, você faria uma sincronização total inicial e, logo depois, obteria periodicamente alterações incrementais para esse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="dea8c-110">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="dea8c-111">Para obter as respostas de uma mensagem, utilize use a operação [listar respostas da mensagem](channel-get-messagereply.md) ou a operação [obter resposta da mensagem](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="dea8c-111">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="dea8c-112">Uma solicitação GET com a função delta traz como resultado uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="dea8c-112">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="dea8c-113">Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou</span><span class="sxs-lookup"><span data-stu-id="dea8c-113">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="dea8c-114">Uma `deltaLink` (que contém uma URL com uma chamada de função **delta** e `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="dea8c-114">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="dea8c-115">Os tokens de estado são completamente opacos para o cliente.</span><span class="sxs-lookup"><span data-stu-id="dea8c-115">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="dea8c-116">Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função delta do mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="dea8c-116">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="dea8c-117">Um `deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída.</span><span class="sxs-lookup"><span data-stu-id="dea8c-117">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="dea8c-118">Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="dea8c-118">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="dea8c-119">Para obter mais informações, consulte a documentação da [consulta Delta](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="dea8c-119">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="dea8c-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="dea8c-120">Permissions</span></span>

<span data-ttu-id="dea8c-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dea8c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="dea8c-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dea8c-123">Permission Type</span></span>                        |<span data-ttu-id="dea8c-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dea8c-124">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="dea8c-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dea8c-125">Delegated (work or school account)</span></span>     |<span data-ttu-id="dea8c-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea8c-126">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="dea8c-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dea8c-127">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dea8c-128">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dea8c-128">Not Supported</span></span>                                |
|<span data-ttu-id="dea8c-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dea8c-129">Application</span></span>                            |<span data-ttu-id="dea8c-130">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea8c-130">Group.Read.All, Group.ReadWrite.All</span></span>          |

> [!NOTE]
> <span data-ttu-id="dea8c-131">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dea8c-131">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="dea8c-132">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="dea8c-132">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="dea8c-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dea8c-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="dea8c-134">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="dea8c-134">Query parameters</span></span>

<span data-ttu-id="dea8c-135">O controle de alterações nas mensagens de canal gera uma série de uma ou mais chamadas de função **delta**.</span><span class="sxs-lookup"><span data-stu-id="dea8c-135">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="dea8c-136">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="dea8c-136">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="dea8c-137">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="dea8c-137">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="dea8c-138">Você só precisa especificar uma vez antecipadamente os parâmetros de consulta desejados.</span><span class="sxs-lookup"><span data-stu-id="dea8c-138">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="dea8c-139">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="dea8c-139">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="dea8c-140">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="dea8c-140">Query parameter</span></span>      | <span data-ttu-id="dea8c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="dea8c-141">Type</span></span>   |<span data-ttu-id="dea8c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="dea8c-142">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="dea8c-143">string</span><span class="sxs-lookup"><span data-stu-id="dea8c-143">string</span></span> | <span data-ttu-id="dea8c-144">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior, indicando a conclusão daquela série de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="dea8c-144">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="dea8c-145">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="dea8c-145">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="dea8c-146">string</span><span class="sxs-lookup"><span data-stu-id="dea8c-146">string</span></span> | <span data-ttu-id="dea8c-147">Um[ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas.</span><span class="sxs-lookup"><span data-stu-id="dea8c-147">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="dea8c-148">Parâmetros de consulta OData opcionais</span><span class="sxs-lookup"><span data-stu-id="dea8c-148">Optional OData query parameters</span></span>

<span data-ttu-id="dea8c-149">Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatível com esta API:</span><span class="sxs-lookup"><span data-stu-id="dea8c-149">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="dea8c-150">`$top`representa o número máximo de mensagens a buscar em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="dea8c-150">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="dea8c-151">O limite máximo é **50**.</span><span class="sxs-lookup"><span data-stu-id="dea8c-151">The upper limit is **50**.</span></span>
- <span data-ttu-id="dea8c-152">`$skip`representa quantas mensagens devem ser ignoradas no início da lista.</span><span class="sxs-lookup"><span data-stu-id="dea8c-152">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="dea8c-153">`$filter` permite retornar mensagens que atendem a certos critérios.</span><span class="sxs-lookup"><span data-stu-id="dea8c-153">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="dea8c-154">A única propriedade que permite a filtragem é `lastModifiedDateTime`, e somente os operadores **gt** são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="dea8c-154">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="dea8c-155">Por exemplo, o`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` vai buscar todas as mensagens criadas ou alteradas após o período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="dea8c-155">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea8c-156">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-156">Request headers</span></span>
| <span data-ttu-id="dea8c-157">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dea8c-157">Header</span></span>        | <span data-ttu-id="dea8c-158">Valor</span><span class="sxs-lookup"><span data-stu-id="dea8c-158">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="dea8c-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="dea8c-159">Authorization</span></span> | <span data-ttu-id="dea8c-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dea8c-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dea8c-162">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dea8c-162">Content-Type</span></span>  | <span data-ttu-id="dea8c-163">application/json</span><span class="sxs-lookup"><span data-stu-id="dea8c-163">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="dea8c-164">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-164">Request Body</span></span>

<span data-ttu-id="dea8c-165">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dea8c-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea8c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="dea8c-166">Response</span></span>

<span data-ttu-id="dea8c-167">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dea8c-167">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="dea8c-168">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="dea8c-168">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="dea8c-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dea8c-169">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="dea8c-170">Exemplo 1: sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="dea8c-170">Example 1: Initial synchronization</span></span>

<span data-ttu-id="dea8c-171">O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens num dado canal.</span><span class="sxs-lookup"><span data-stu-id="dea8c-171">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="dea8c-172">Há cinco mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="dea8c-172">There are five messages in the channel.</span></span>

- <span data-ttu-id="dea8c-173">Etapa 1:[ exemplo inicial de solicitação](#initial-request) e [resposta](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="dea8c-173">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="dea8c-174">Etapa 2:[ segundo exemplo de solicitação](#second-request) e [resposta](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="dea8c-174">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="dea8c-175">Etapa 3:[ terceiro exemplo de solicitação](#third-request) e [resposta final](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="dea8c-175">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="dea8c-p115">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="dea8c-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="dea8c-178">Confira também o que você vai fazer na [próxima fase](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="dea8c-178">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="dea8c-179">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="dea8c-179">Initial request</span></span>

<span data-ttu-id="dea8c-180">Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto a solicitação de sincronização inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="dea8c-180">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="dea8c-181">Essa rodada mostrará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="dea8c-181">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="dea8c-182">A solicitação especifica o cabeçalho de solicitação opcional, odata.top, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="dea8c-182">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dea8c-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea8c-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dea8c-184">C#</span><span class="sxs-lookup"><span data-stu-id="dea8c-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dea8c-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea8c-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dea8c-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea8c-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="dea8c-187">Resposta inicial da solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-187">Initial request response</span></span>

<span data-ttu-id="dea8c-188">A resposta inclui duas mensagens e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="dea8c-188">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="dea8c-189">A URL `nextLink` indica que há mais mensagens na pasta a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="dea8c-189">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="dea8c-190">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dea8c-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dea8c-191">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dea8c-191">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="dea8c-192">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-192">Second request</span></span>

<span data-ttu-id="dea8c-193">A segunda solicitação especifica a URL `nextLink` retornada na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="dea8c-193">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="dea8c-194">Observe que não é mais necessário especificar os mesmos parâmetros principais definidos na solicitação inicial, pois o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="dea8c-194">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dea8c-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea8c-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dea8c-196">C#</span><span class="sxs-lookup"><span data-stu-id="dea8c-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dea8c-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea8c-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dea8c-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea8c-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="dea8c-199">Resposta da segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-199">Second request response</span></span>

<span data-ttu-id="dea8c-200">A segunda resposta retorna as 2 próximas mensagens e um `@odata.nextLink` cabeçalho de resposta com um`skipToken`, indicando que há mais mensagens para se obter no canal.</span><span class="sxs-lookup"><span data-stu-id="dea8c-200">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="dea8c-201">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dea8c-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dea8c-202">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dea8c-202">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="dea8c-203">Terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-203">Third request</span></span>

<span data-ttu-id="dea8c-204">A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="dea8c-204">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dea8c-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea8c-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dea8c-206">C#</span><span class="sxs-lookup"><span data-stu-id="dea8c-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dea8c-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea8c-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dea8c-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea8c-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="dea8c-209">Resposta da terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-209">Third request response</span></span>

<span data-ttu-id="dea8c-210">A terceira resposta retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas.</span><span class="sxs-lookup"><span data-stu-id="dea8c-210">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="dea8c-211">Salvar e usar a URL `deltaLink` para consultar novas mensagens a partir desse ponto na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="dea8c-211">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="dea8c-212">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dea8c-212">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dea8c-213">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dea8c-213">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="dea8c-214">Exemplo 2: recuperar alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="dea8c-214">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="dea8c-215">Usando o `deltaLink` da última solicitação na última fase, você poderá obter somente as mensagens que sofreram alteração (por terem sido adicionadas, excluídas ou atualizadas) nesse canal desde então.</span><span class="sxs-lookup"><span data-stu-id="dea8c-215">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="dea8c-216">Supondo que você prefira manter o mesmo tamanho máximo de página na resposta, sua solicitação terá um formato semelhante a este :</span><span class="sxs-lookup"><span data-stu-id="dea8c-216">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="dea8c-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dea8c-217">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dea8c-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea8c-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dea8c-219">C#</span><span class="sxs-lookup"><span data-stu-id="dea8c-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dea8c-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea8c-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dea8c-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea8c-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dea8c-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="dea8c-222">Response</span></span>

><span data-ttu-id="dea8c-p124">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dea8c-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
