---
title: 'chatMessage: delta'
description: Recupere a lista de mensagens (sem as respostas) em um canal de uma equipe. Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.
localization_priority: Priority
doc_type: apiPageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e24106814dac97a8585245a48a3f1641c98188d7
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582680"
---
# <a name="chatmessage-delta"></a><span data-ttu-id="eece0-104">chatMessage: delta</span><span class="sxs-lookup"><span data-stu-id="eece0-104">chatMessage: delta</span></span>

<span data-ttu-id="eece0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eece0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eece0-106">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="eece0-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="eece0-107">Usando a consulta Delta, você pode obter mensagens novas ou atualizadas em um canal.</span><span class="sxs-lookup"><span data-stu-id="eece0-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="eece0-108">**Observação:** Delta retornará apenas as mensagens dos últimos oito meses.</span><span class="sxs-lookup"><span data-stu-id="eece0-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="eece0-109">Você pode usar [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) para recuperar mensagens mais antigas.</span><span class="sxs-lookup"><span data-stu-id="eece0-109">You can use [GET /teams/{team-id}/channels/{channel-id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="eece0-110">A consulta Delta é compatível tanto com sincronização completa que recupera todos as mensagens num canal especificado quanto com a sincronização incremental que recupera as mensagens que foram adicionadas ou alteradas no canal desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="eece0-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="eece0-111">Normalmente, você faria uma sincronização total inicial e, logo depois, obteria periodicamente alterações incrementais para esse modo de exibição de mensagens.</span><span class="sxs-lookup"><span data-stu-id="eece0-111">Typically, you would do an initial full synchronization, and then get incremental changes to that messages view periodically.</span></span>

<span data-ttu-id="eece0-112">Para obter as respostas de uma mensagem, utilize use a operação [listar respostas da mensagem](chatmessage-list-replies.md) ou a operação [obter resposta da mensagem](chatmessage-get.md).</span><span class="sxs-lookup"><span data-stu-id="eece0-112">To get the replies for a message, use the [list message replies](chatmessage-list-replies.md) or the [get message reply](chatmessage-get.md) operation.</span></span>

<span data-ttu-id="eece0-113">Uma solicitação GET com a função delta traz como resultado uma destas opções:</span><span class="sxs-lookup"><span data-stu-id="eece0-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="eece0-114">Uma `nextLink` (que contém uma URL com uma chamada de função **delta** e uma `skipToken`) ou</span><span class="sxs-lookup"><span data-stu-id="eece0-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="eece0-115">Uma `deltaLink` (que contém uma URL com uma chamada de função **delta** e `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="eece0-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="eece0-116">Os tokens de estado são completamente opacos para o cliente.</span><span class="sxs-lookup"><span data-stu-id="eece0-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="eece0-117">Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função delta do mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="eece0-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="eece0-118">Um `deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída.</span><span class="sxs-lookup"><span data-stu-id="eece0-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="eece0-119">Você pode salvar e usar a URL `deltaLink` quando começar a recuperar alterações adicionais (mensagens alteradas ou postadas após a aquisição de `deltaLink`).</span><span class="sxs-lookup"><span data-stu-id="eece0-119">You can save and use the `deltaLink` URL when you begin the to retrieve additional changes (messages changed or posted after acquiring `deltaLink`).</span></span>

<span data-ttu-id="eece0-120">Para obter mais informações, consulte a documentação da [consulta Delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="eece0-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="eece0-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="eece0-121">Permissions</span></span>

<span data-ttu-id="eece0-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eece0-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="eece0-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eece0-124">Permission Type</span></span>                        |<span data-ttu-id="eece0-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eece0-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="eece0-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eece0-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="eece0-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eece0-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="eece0-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eece0-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eece0-129">Não suportado</span><span class="sxs-lookup"><span data-stu-id="eece0-129">Not Supported</span></span>                                |
|<span data-ttu-id="eece0-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eece0-130">Application</span></span>                            | <span data-ttu-id="eece0-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eece0-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="eece0-132">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="eece0-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="eece0-133">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eece0-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="eece0-134">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="eece0-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="eece0-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eece0-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="eece0-136">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="eece0-136">Query parameters</span></span>

<span data-ttu-id="eece0-137">O controle de alterações nas mensagens de canal gera uma série de uma ou mais chamadas de função **delta**.</span><span class="sxs-lookup"><span data-stu-id="eece0-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="eece0-138">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="eece0-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="eece0-139">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="eece0-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="eece0-140">Você só precisa especificar uma vez antecipadamente os parâmetros de consulta desejados.</span><span class="sxs-lookup"><span data-stu-id="eece0-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="eece0-141">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="eece0-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="eece0-142">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="eece0-142">Query parameter</span></span>      | <span data-ttu-id="eece0-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="eece0-143">Type</span></span>   |<span data-ttu-id="eece0-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="eece0-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="eece0-145">string</span><span class="sxs-lookup"><span data-stu-id="eece0-145">string</span></span> | <span data-ttu-id="eece0-146">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior, indicando a conclusão daquela série de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="eece0-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="eece0-147">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima iteração de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="eece0-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next iteration of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="eece0-148">string</span><span class="sxs-lookup"><span data-stu-id="eece0-148">string</span></span> | <span data-ttu-id="eece0-149">Um [ token de estado](/graph/delta-query-overview) retornado na URL`nextLink` da chamada de função **delta** anterior indicando que há mais alterações a serem controladas.</span><span class="sxs-lookup"><span data-stu-id="eece0-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="eece0-150">Parâmetros de consulta OData opcionais</span><span class="sxs-lookup"><span data-stu-id="eece0-150">Optional OData query parameters</span></span>

<span data-ttu-id="eece0-151">Os seguintes [parâmetros de consulta OData](/graph/query-parameters) são compatível com esta API:</span><span class="sxs-lookup"><span data-stu-id="eece0-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="eece0-152">`$top`representa o número máximo de mensagens a buscar em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="eece0-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="eece0-153">O limite máximo é **50**.</span><span class="sxs-lookup"><span data-stu-id="eece0-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="eece0-154">`$skip`representa quantas mensagens devem ser ignoradas no início da lista.</span><span class="sxs-lookup"><span data-stu-id="eece0-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="eece0-155">`$filter` permite retornar mensagens que atendem a certos critérios.</span><span class="sxs-lookup"><span data-stu-id="eece0-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="eece0-156">A única propriedade que permite a filtragem é `lastModifiedDateTime`, e somente os operadores **gt** são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="eece0-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="eece0-157">Por exemplo, o`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` vai buscar todas as mensagens criadas ou alteradas após o período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="eece0-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eece0-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-158">Request headers</span></span>
| <span data-ttu-id="eece0-159">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eece0-159">Header</span></span>        | <span data-ttu-id="eece0-160">Valor</span><span class="sxs-lookup"><span data-stu-id="eece0-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="eece0-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="eece0-161">Authorization</span></span> | <span data-ttu-id="eece0-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eece0-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eece0-164">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-164">Request Body</span></span>

<span data-ttu-id="eece0-165">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eece0-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eece0-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="eece0-166">Response</span></span>

<span data-ttu-id="eece0-167">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eece0-167">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="eece0-168">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="eece0-168">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="eece0-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eece0-169">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="eece0-170">Exemplo 1: sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="eece0-170">Example 1: Initial synchronization</span></span>

<span data-ttu-id="eece0-171">O exemplo a seguir mostra uma série de três solicitações para sincronizar as mensagens num dado canal.</span><span class="sxs-lookup"><span data-stu-id="eece0-171">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="eece0-172">Há cinco mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="eece0-172">There are five messages in the channel.</span></span>

- <span data-ttu-id="eece0-173">Etapa 1:[solicitação inicial](#initial-request) e [resposta](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="eece0-173">Step 1: [initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="eece0-174">Etapa 2:[segunda solicitação](#second-request) e [resposta](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="eece0-174">Step 2: [second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="eece0-175">Etapa 3:[terceira solicitação](#third-request) e [resposta final](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="eece0-175">Step 3: [third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="eece0-p115">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="eece0-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="eece0-178">Veja também o que poderá fazer [para recuperar alterações adicionais](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="eece0-178">See also what you'll do [to retrieve additional changes](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="eece0-179">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="eece0-179">Initial request</span></span>

<span data-ttu-id="eece0-180">Neste exemplo, as mensagens do canal estão sendo sincronizadas pela primeira vez, portanto a solicitação de sincronização inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="eece0-180">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="eece0-181">Essa rodada mostrará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="eece0-181">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="eece0-182">A solicitação especifica o cabeçalho de solicitação opcional, odata.top, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="eece0-182">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_1"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$top=2
```

#### <a name="initial-request-response"></a><span data-ttu-id="eece0-183">Resposta inicial da solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-183">Initial request response</span></span>

<span data-ttu-id="eece0-184">A resposta inclui duas mensagens e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="eece0-184">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="eece0-185">A URL `nextLink` indica que há mais mensagens na pasta a serem obtidas.</span><span class="sxs-lookup"><span data-stu-id="eece0-185">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606515483514",
            "messageType": "message",
            "createdDateTime": "2020-11-27T22:18:03.514Z",
            "lastModifiedDateTime": "2020-11-27T22:18:03.514Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606515483514?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606515483514&parentMessageId=1606515483514",
            "policyViolation": null,
            "id": "1606515483514",
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
                "content": "Test"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691795113",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:35.113Z",
            "lastModifiedDateTime": "2020-11-29T23:16:35.113Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691795113?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691795113&parentMessageId=1606691795113",
            "policyViolation": null,
            "id": "1606691795113",
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
                "content": "HelloWorld 11/29/2020 3:16:31 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="second-request"></a><span data-ttu-id="eece0-186">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-186">Second request</span></span>

<span data-ttu-id="eece0-187">A segunda solicitação especifica a URL `nextLink` retornada na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="eece0-187">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="eece0-188">Observe que não é mais necessário especificar os mesmos parâmetros principais definidos na solicitação inicial, pois o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="eece0-188">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_2"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58
```

#### <a name="second-request-response"></a><span data-ttu-id="eece0-189">Resposta da segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-189">Second request response</span></span>

<span data-ttu-id="eece0-190">A segunda resposta retorna as 2 próximas mensagens e um `@odata.nextLink` cabeçalho de resposta com um`skipToken`, indicando que há mais mensagens para se obter no canal.</span><span class="sxs-lookup"><span data-stu-id="eece0-190">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691812117",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:52.117Z",
            "lastModifiedDateTime": "2020-11-29T23:16:52.117Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691812117?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691812117&parentMessageId=1606691812117",
            "policyViolation": null,
            "id": "1606691812117",
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
                "content": "HelloWorld 11/29/2020 3:16:51 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691846203",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:17:26.203Z",
            "lastModifiedDateTime": "2020-11-29T23:17:26.203Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691846203?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691846203&parentMessageId=1606691846203",
            "policyViolation": null,
            "id": "1606691846203",
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
                "content": "HelloWorld 11/29/2020 3:17:25 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="third-request"></a><span data-ttu-id="eece0-191">Terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-191">Third request</span></span>

<span data-ttu-id="eece0-192">A terceira solicitação continua a usar a URL `nextLink` mais recente retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="eece0-192">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_3"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4
```

#### <a name="third-request-response"></a><span data-ttu-id="eece0-193">Resposta da terceira solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-193">Third request response</span></span>

<span data-ttu-id="eece0-194">A terceira resposta retorna as únicas mensagens restantes no canal e um `@odata.deltaLink` cabeçalho de resposta com um `deltaToken` que indica que todas as mensagens no canal foram lidas.</span><span class="sxs-lookup"><span data-stu-id="eece0-194">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="eece0-195">Salve e use a URL `deltaLink` para consultar novas mensagens a partir desse ponto em diante.</span><span class="sxs-lookup"><span data-stu-id="eece0-195">Save and use the `deltaLink` URL to query for any new messages starting from this point onwards.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351582080",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:39:42.08Z",
            "lastModifiedDateTime": "2021-01-22T21:39:42.08Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351582080?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351582080&parentMessageId=1611351582080",
            "policyViolation": null,
            "id": "1611351582080",
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
                "content": "HelloWorld 1/22/2021 1:39:39 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351603178",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:40:03.178Z",
            "lastModifiedDateTime": "2021-01-22T21:40:03.178Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351603178?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351603178&parentMessageId=1611351603178",
            "policyViolation": null,
            "id": "1611351603178",
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
                "content": "HelloWorld 1/22/2021 1:40:00 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="eece0-196">Exemplo 2: recuperar alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="eece0-196">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="eece0-197">Usando o `deltaLink` da última solicitação na última fase, você poderá obter somente as mensagens que sofreram alteração (por terem sido adicionadas, excluídas ou atualizadas) nesse canal desde então.</span><span class="sxs-lookup"><span data-stu-id="eece0-197">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="eece0-198">Supondo que você prefira manter o mesmo tamanho máximo de página na resposta, sua solicitação terá um formato semelhante a este :</span><span class="sxs-lookup"><span data-stu-id="eece0-198">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="eece0-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-199">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_4"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4
```

#### <a name="response"></a><span data-ttu-id="eece0-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="eece0-200">Response</span></span>

><span data-ttu-id="eece0-p121">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eece0-p121">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_yjz2nsMoh1gXNtXii7s78HapCi5woifXqwXlVNxICh8wUUnvE2gExsa8eZ2Vy_ch5rVIhm067_1mUPML3iYUVyg.3o0rhgaBUduuxOr98An5pjBDP5JjKUiVWku3flSiOsk",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1616989510408",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:45:10.408Z",
            "lastModifiedDateTime": "2021-03-29T03:45:10.408Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989510408?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989510408&parentMessageId=1616989510408",
            "policyViolation": null,
            "id": "1616989510408",
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
                "content": "Hello World 28th March 2021"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
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


