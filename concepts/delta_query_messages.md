# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="c5313-101">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="c5313-101">Get incremental changes to messages in a folder</span></span> 

<span data-ttu-id="c5313-p101">A consulta delta permite consultar adições, exclusões ou atualizações de mensagens em uma pasta, por meio de uma série de chamadas de função [delta](../api-reference/v1.0/api/message_delta.md). Os dados delta permitem manter e sincronizar um armazenamento local de mensagens do usuário, sem ter de buscar todo o conjunto de mensagens do usuário no servidor a cada vez que precise deles.</span><span class="sxs-lookup"><span data-stu-id="c5313-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="c5313-p102">A consulta delta oferece suporte à sincronização completa, que recupera todas as mensagens em uma pasta (por exemplo, a Caixa de Entrada do usuário), e à sincronização incremental, que recupera todas as mensagens que foram alteradas nessa pasta desde a última sincronização. Normalmente, você faria uma sincronização completa inicial de todas as mensagens em uma pasta e, logo após, obteria alterações incrementais para essa pasta periodicamente.</span><span class="sxs-lookup"><span data-stu-id="c5313-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span> 

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="c5313-106">Controlar mensagens de alterações em uma pasta</span><span class="sxs-lookup"><span data-stu-id="c5313-106">Track message changes in a folder</span></span>

<span data-ttu-id="c5313-p103">A consulta delta é uma operação por pasta. Para controlar as alterações das mensagens em uma hierarquia de pastas, você precisa controlar cada pasta individualmente.</span><span class="sxs-lookup"><span data-stu-id="c5313-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span> 

<span data-ttu-id="c5313-p104">O rastreamento de alterações de mensagem em uma paste de email corresponde a uma série de solicitações GET com a função **delta**. A solicitação GET inicial é muito semelhante à maneira como você [obtém mensagens](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), exceto se você incluir a função **delta**:</span><span class="sxs-lookup"><span data-stu-id="c5313-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="c5313-111">Uma solicitação GET com a função **delta** retorna:</span><span class="sxs-lookup"><span data-stu-id="c5313-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="c5313-112">Uma `nextLink` (que contém uma URL com chamada de função **delta** e um _skipToken_) ou</span><span class="sxs-lookup"><span data-stu-id="c5313-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="c5313-113">Uma `deltaLink` (que contém uma URL com chamada de função **delta** e _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="c5313-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="c5313-p105">Esses tokens são [tokens de estado](delta_query_overview.md#state-tokens) que são completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL retornada da última solicitação GET para a próxima chamada de função **delta** da mesma pasta. Um `deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="c5313-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="c5313-118">Verifique o [exemplo](#example-to-synchronize-messages-in-a-folder) abaixo para aprender a usar as URLs `nextLink` e `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="c5313-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="c5313-119">Use os parâmetros de consulta em uma consulta delta para mensagens</span><span class="sxs-lookup"><span data-stu-id="c5313-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="c5313-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="c5313-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="c5313-122">Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens.</span><span class="sxs-lookup"><span data-stu-id="c5313-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="c5313-123">Há suporte limitado para `$filter` e `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="c5313-123">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="c5313-124">As únicas expressões `$filter` suportadas são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="c5313-124">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="c5313-p107">A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.</span><span class="sxs-lookup"><span data-stu-id="c5313-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="c5313-127">Não há suporte DAV para `$search`.</span><span class="sxs-lookup"><span data-stu-id="c5313-127">There is no support for `$search`.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="c5313-128">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c5313-128">Optional request header</span></span>

<span data-ttu-id="c5313-129">Cada solicitação GET de consulta delta retorna um conjunto de um ou mais mensagens na resposta.</span><span class="sxs-lookup"><span data-stu-id="c5313-129">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, Prefer: odata.maxpagesize={x}, to set the maximum number of messages in a response.</span></span> <span data-ttu-id="c5313-130">Como alternativa, você pode especificar o cabeçalho de solicitação, `Prefer: odata.maxpagesize={x}`, para configurar o máximo de mensagens em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c5313-130">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of messages in a response.</span></span>

<!--
### Iterative process 

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query 
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative 
process (steps 2-6) described below will return the entire set of messages in that folder. 

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header, 
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned 
   in _@odata.nextLink_, which includes a _skipToken_. 

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages, 
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3. 

6. When you eventually receive a _detlaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This 
round of change tracking is complete. 

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request 
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated) 
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="c5313-131">Exemplo para sincronizar mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="c5313-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="c5313-132">O exemplo a seguir mostra uma série de 3 solicitações para sincronizar uma pasta específica contendo 5 mensagens:</span><span class="sxs-lookup"><span data-stu-id="c5313-132">The following example shows a series of 3 requests to synchronize a specific folder which contains 5 messages:</span></span>

- <span data-ttu-id="c5313-133">[Solicitação inicial de exemplo](#sample-initial-request) e [resposta](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="c5313-133">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="c5313-134">[Solicitação de segundo exemplo](#sample-second-request) e [resposta](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="c5313-134">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="c5313-135">[Terceiro exemplo de solicitação](#sample-third-request) e [resposta final](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="c5313-135">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="c5313-136">Confira também o que você vai fazer na [próxima fase](#the-next-round).</span><span class="sxs-lookup"><span data-stu-id="c5313-136">See also what you'll do in the [next round](#the-next-round).</span></span>


### <a name="sample-initial-request"></a><span data-ttu-id="c5313-137">Solicitação inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="c5313-137">Sample initial request</span></span>

<span data-ttu-id="c5313-p109">Neste exemplo,a pasta especificada está sendo sincronizada pela primeira vez, para que a solicitação de sincronização inicial não inclua nenhum token de estado. Esta fase retornará todas as mensagens nessa pasta.</span><span class="sxs-lookup"><span data-stu-id="c5313-p109">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="c5313-140">A primeira solicitação especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5313-140">The first request specifies the following:</span></span>

- <span data-ttu-id="c5313-141">Um parâmetro `$select` para retornar as propriedades de **Subject** e **Sender** de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="c5313-141">A `$select` parameter to return the **Subject** and **Sender** properties for each message in the response.</span></span>
- <span data-ttu-id="c5313-142">O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 mensagens de cada vez.</span><span class="sxs-lookup"><span data-stu-id="c5313-142">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="c5313-143">Resposta inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="c5313-143">Sample initial response</span></span>

<span data-ttu-id="c5313-p110">A resposta inclui duas mensagens e um cabeçalho de resposta `@odata.nextLink`. A URL `nextLink` indica que há mais mensagens na pasta para obter.</span><span class="sxs-lookup"><span data-stu-id="c5313-p110">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
            "subject":"Holiday hours update",
            "sender":{
                "emailAddress":{
                    "name":"Dana Swope",
                    "address":"danas@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADNkNAAASq35xAAA="
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
            "subject":"Holiday promotion sale",
            "sender":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAVRMKAAAAA=="
        }
    ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="c5313-146">Segundo exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5313-146">Sample second request</span></span>

<span data-ttu-id="c5313-p111">A segunda solicitação especifica a URL `nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar o mesmo parâmetro `$select` como na solicitação inicial, pois o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="c5313-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="c5313-149">Segunda resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="c5313-149">Sample second response</span></span> 

<span data-ttu-id="c5313-150">A segunda resposta retorna as 2 próximas mensagens na pasta e outro `nextLink`, indicando que há mais mensagens a ser lidas na pasta.</span><span class="sxs-lookup"><span data-stu-id="c5313-150">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWJAAAA"
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB9\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWHAAAA"
        }
    ]
}
```


### <a name="sample-third-request"></a><span data-ttu-id="c5313-151">Terceira solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="c5313-151">Sample third request</span></span>

<span data-ttu-id="c5313-152">A terceira solicitação continua a usar a última URL do `nextLink` retornada da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c5313-152">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="c5313-153">Terceira e última resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="c5313-153">Sample third and final response</span></span>

<span data-ttu-id="c5313-p112">A terceira resposta retorna a única mensagem restante em uma pasta, e uma URL `deltaLink` que indica que a sincronização está, por enquanto, concluída para esta pasta. Salvar e usar a URL `deltaLink` para [sincronizar a mesma pasta na próxima fase](#the-next-round).</span><span class="sxs-lookup"><span data-stu-id="c5313-p112">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB8\"",
            "subject":"You've joined the Customer Manager group",
            "sender":{
                "emailAddress":{
                    "name":"Customer Managers team",
                    "address":"customer_managers@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWFAAAA"
        }
    ]
}
```


### <a name="the-next-round"></a><span data-ttu-id="c5313-156">A próxima fase</span><span class="sxs-lookup"><span data-stu-id="c5313-156">The next round</span></span>

<span data-ttu-id="c5313-p113">Usando o `deltaLink` da [última solicitação](#sample-third-request) na última fase, você poderá obter somente as mensagens que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse nessa pasta desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:</span><span class="sxs-lookup"><span data-stu-id="c5313-p113">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a><span data-ttu-id="c5313-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5313-159">See also</span></span>

- [<span data-ttu-id="c5313-160">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c5313-160">Microsoft Graph delta query</span></span>](../Concepts/delta_query_overview.md)
- [<span data-ttu-id="c5313-161">Obter as alterações incrementais para os eventos em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="c5313-161">Get incremental changes to events in a calendar view</span></span>](../Concepts/delta_query_events.md)
- [<span data-ttu-id="c5313-162">Obter as alterações incrementais para grupos</span><span class="sxs-lookup"><span data-stu-id="c5313-162">Get incremental changes to groups</span></span>](../Concepts/delta_query_groups.md)
- [<span data-ttu-id="c5313-163">Obter as alterações incrementais para usuários</span><span class="sxs-lookup"><span data-stu-id="c5313-163">Get incremental changes to users</span></span>](../Concepts/delta_query_users.md)
