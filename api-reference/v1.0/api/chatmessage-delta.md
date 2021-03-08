---
title: 'chatMessages: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: c1282d71fbd0ae51f4ce1a24549ca2721c77a260
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515657"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="72f5a-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="72f5a-104">chatMessages: delta</span></span>

<span data-ttu-id="72f5a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f5a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72f5a-106">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="72f5a-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="72f5a-107">Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.</span><span class="sxs-lookup"><span data-stu-id="72f5a-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="72f5a-108">**Observação:** Delta retornará apenas as mensagens dos últimos oito meses.</span><span class="sxs-lookup"><span data-stu-id="72f5a-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="72f5a-109">Você pode usar [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) para recuperar mensagens mais antigas.</span><span class="sxs-lookup"><span data-stu-id="72f5a-109">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="72f5a-110">A consulta Delta é compatível tanto com sincronização completa que recupera todos as mensagens num canal especificado quanto com a sincronização incremental que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="72f5a-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="72f5a-111">Normalmente, você faria uma sincronização total inicial e, logo depois, obteria periodicamente alterações incrementais para esse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="72f5a-111">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="72f5a-112">Para obter as respostas de uma mensagem, utilize use a operação [listar respostas da mensagem](channel-get-messagereply.md) ou a operação [obter resposta da mensagem](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="72f5a-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="72f5a-113">Uma solicitação GET com a função delta traz como resultado uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="72f5a-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="72f5a-114">Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou</span><span class="sxs-lookup"><span data-stu-id="72f5a-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="72f5a-115">Uma `deltaLink` (que contém uma URL com uma chamada de função **delta** e `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="72f5a-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="72f5a-116">Os tokens de estado são completamente opacos para o cliente.</span><span class="sxs-lookup"><span data-stu-id="72f5a-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="72f5a-117">Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função delta do mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="72f5a-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="72f5a-118">Um `deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída.</span><span class="sxs-lookup"><span data-stu-id="72f5a-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="72f5a-119">Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="72f5a-119">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="72f5a-120">Para obter mais informações, consulte a documentação da [consulta Delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="72f5a-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="72f5a-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="72f5a-121">Permissions</span></span>

<span data-ttu-id="72f5a-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="72f5a-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="72f5a-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72f5a-124">Permission Type</span></span>                        |<span data-ttu-id="72f5a-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72f5a-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="72f5a-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72f5a-126">Delegated (work or school account)</span></span>| <span data-ttu-id="72f5a-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="72f5a-127">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="72f5a-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72f5a-128">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72f5a-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72f5a-129">Not supported.</span></span>|
|<span data-ttu-id="72f5a-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72f5a-130">Application</span></span>| <span data-ttu-id="72f5a-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="72f5a-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="72f5a-132">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="72f5a-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="72f5a-133">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72f5a-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="72f5a-134">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="72f5a-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="72f5a-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72f5a-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="72f5a-136">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="72f5a-136">Query parameters</span></span>

<span data-ttu-id="72f5a-137">O controle de alterações nas mensagens de canal gera uma série de uma ou mais chamadas de função **delta**.</span><span class="sxs-lookup"><span data-stu-id="72f5a-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="72f5a-138">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="72f5a-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="72f5a-139">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="72f5a-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="72f5a-140">Você só precisa especificar uma vez antecipadamente os parâmetros de consulta desejados.</span><span class="sxs-lookup"><span data-stu-id="72f5a-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="72f5a-141">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="72f5a-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="72f5a-142">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="72f5a-142">Query parameter</span></span>      | <span data-ttu-id="72f5a-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="72f5a-143">Type</span></span>   |<span data-ttu-id="72f5a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="72f5a-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="72f5a-145">string</span><span class="sxs-lookup"><span data-stu-id="72f5a-145">string</span></span> | <span data-ttu-id="72f5a-146">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior, indicando a conclusão daquela série de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="72f5a-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="72f5a-147">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="72f5a-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="72f5a-148">string</span><span class="sxs-lookup"><span data-stu-id="72f5a-148">string</span></span> | <span data-ttu-id="72f5a-149">Um [ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas.</span><span class="sxs-lookup"><span data-stu-id="72f5a-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="72f5a-150">Parâmetros de consulta OData opcionais</span><span class="sxs-lookup"><span data-stu-id="72f5a-150">Optional OData query parameters</span></span>

<span data-ttu-id="72f5a-151">Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatível com esta API:</span><span class="sxs-lookup"><span data-stu-id="72f5a-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="72f5a-152">`$top`representa o número máximo de mensagens a buscar em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="72f5a-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="72f5a-153">O limite máximo é **50**.</span><span class="sxs-lookup"><span data-stu-id="72f5a-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="72f5a-154">`$skip`representa quantas mensagens devem ser ignoradas no início da lista.</span><span class="sxs-lookup"><span data-stu-id="72f5a-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="72f5a-155">`$filter` permite retornar mensagens que atendem a certos critérios.</span><span class="sxs-lookup"><span data-stu-id="72f5a-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="72f5a-156">A única propriedade que permite a filtragem é `lastModifiedDateTime`, e somente os operadores **gt** são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="72f5a-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="72f5a-157">Por exemplo, o`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` vai buscar todas as mensagens criadas ou alteradas após o período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="72f5a-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72f5a-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-158">Request headers</span></span>
| <span data-ttu-id="72f5a-159">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72f5a-159">Header</span></span>        | <span data-ttu-id="72f5a-160">Valor</span><span class="sxs-lookup"><span data-stu-id="72f5a-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="72f5a-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="72f5a-161">Authorization</span></span> | <span data-ttu-id="72f5a-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72f5a-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72f5a-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72f5a-164">Content-Type</span></span>  | <span data-ttu-id="72f5a-165">application/json</span><span class="sxs-lookup"><span data-stu-id="72f5a-165">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="72f5a-166">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-166">Request Body</span></span>

<span data-ttu-id="72f5a-167">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72f5a-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72f5a-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f5a-168">Response</span></span>

<span data-ttu-id="72f5a-169">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72f5a-169">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="72f5a-170">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="72f5a-170">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="72f5a-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72f5a-171">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="72f5a-172">Exemplo 1: sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="72f5a-172">Example 1: Initial synchronization</span></span>

<span data-ttu-id="72f5a-173">O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens num dado canal.</span><span class="sxs-lookup"><span data-stu-id="72f5a-173">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="72f5a-174">Há cinco mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="72f5a-174">There are five messages in the channel.</span></span>

- <span data-ttu-id="72f5a-175">Etapa 1:[ exemplo inicial de solicitação](#initial-request) e [resposta](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="72f5a-175">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="72f5a-176">Etapa 2:[ segundo exemplo de solicitação](#second-request) e [resposta](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="72f5a-176">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="72f5a-177">Etapa 3:[ terceiro exemplo de solicitação](#third-request) e [resposta final](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="72f5a-177">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="72f5a-p115">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="72f5a-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="72f5a-180">Confira também o que você vai fazer na [próxima fase](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="72f5a-180">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="72f5a-181">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="72f5a-181">Initial request</span></span>

<span data-ttu-id="72f5a-182">Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto a solicitação de sincronização inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="72f5a-182">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="72f5a-183">Essa rodada mostrará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="72f5a-183">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="72f5a-184">A solicitação especifica o cabeçalho de solicitação opcional, odata.top, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="72f5a-184">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>



# <a name="http"></a>[<span data-ttu-id="72f5a-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="72f5a-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="72f5a-186">C#</span><span class="sxs-lookup"><span data-stu-id="72f5a-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72f5a-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72f5a-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72f5a-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72f5a-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72f5a-189">Java</span><span class="sxs-lookup"><span data-stu-id="72f5a-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="initial-request-response"></a><span data-ttu-id="72f5a-190">Resposta inicial da solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-190">Initial request response</span></span>

<span data-ttu-id="72f5a-191">A resposta inclui duas mensagens e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="72f5a-191">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="72f5a-192">A URL `nextLink` indica que há mais mensagens na pasta a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="72f5a-192">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="72f5a-193">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72f5a-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72f5a-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72f5a-194">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="72f5a-195">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-195">Second request</span></span>

<span data-ttu-id="72f5a-196">A segunda solicitação especifica a URL `nextLink` retornada na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="72f5a-196">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="72f5a-197">Observe que não é mais necessário especificar os mesmos parâmetros principais definidos na solicitação inicial, pois o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="72f5a-197">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="72f5a-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="72f5a-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="72f5a-199">C#</span><span class="sxs-lookup"><span data-stu-id="72f5a-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72f5a-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72f5a-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72f5a-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72f5a-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72f5a-202">Java</span><span class="sxs-lookup"><span data-stu-id="72f5a-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="second-request-response"></a><span data-ttu-id="72f5a-203">Resposta da segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-203">Second request response</span></span>

<span data-ttu-id="72f5a-204">A segunda resposta retorna as 2 próximas mensagens e um `@odata.nextLink` cabeçalho de resposta com um`skipToken`, indicando que há mais mensagens para se obter no canal.</span><span class="sxs-lookup"><span data-stu-id="72f5a-204">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="72f5a-205">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72f5a-205">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72f5a-206">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72f5a-206">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="72f5a-207">Terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-207">Third request</span></span>

<span data-ttu-id="72f5a-208">A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="72f5a-208">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>



# <a name="http"></a>[<span data-ttu-id="72f5a-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="72f5a-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="72f5a-210">C#</span><span class="sxs-lookup"><span data-stu-id="72f5a-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72f5a-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72f5a-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72f5a-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72f5a-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72f5a-213">Java</span><span class="sxs-lookup"><span data-stu-id="72f5a-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="third-request-response"></a><span data-ttu-id="72f5a-214">Resposta da terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-214">Third request response</span></span>

<span data-ttu-id="72f5a-215">A terceira resposta retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas.</span><span class="sxs-lookup"><span data-stu-id="72f5a-215">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="72f5a-216">Salvar e usar a URL `deltaLink` para consultar novas mensagens a partir desse ponto na próxima rodada.</span><span class="sxs-lookup"><span data-stu-id="72f5a-216">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="72f5a-217">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72f5a-217">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72f5a-218">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72f5a-218">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="72f5a-219">Exemplo 2: recuperar alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="72f5a-219">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="72f5a-220">Usando o `deltaLink` da última solicitação na última fase, você poderá obter somente as mensagens que sofreram alteração (por terem sido adicionadas, excluídas ou atualizadas) nesse canal desde então.</span><span class="sxs-lookup"><span data-stu-id="72f5a-220">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="72f5a-221">Supondo que você prefira manter o mesmo tamanho máximo de página na resposta, sua solicitação terá um formato semelhante a este :</span><span class="sxs-lookup"><span data-stu-id="72f5a-221">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="72f5a-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72f5a-222">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="72f5a-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="72f5a-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="72f5a-224">C#</span><span class="sxs-lookup"><span data-stu-id="72f5a-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72f5a-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72f5a-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72f5a-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72f5a-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72f5a-227">Java</span><span class="sxs-lookup"><span data-stu-id="72f5a-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="72f5a-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f5a-228">Response</span></span>

><span data-ttu-id="72f5a-p124">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72f5a-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


