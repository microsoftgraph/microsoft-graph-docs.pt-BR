---
title: 'message: delta'
description: Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d31efa462d0e4c57f9be32be15838cc5be816ed8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128250"
---
# <a name="message-delta"></a><span data-ttu-id="ba410-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="ba410-103">message: delta</span></span>

<span data-ttu-id="ba410-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba410-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba410-105">Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ba410-105">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="ba410-p101">Uma chamada de função **delta** de mensagens em uma pasta é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite [consultar alterações incrementais nas mensagens dessa pasta](/graph/delta-query-messages). Isso permite manter e sincronizar um armazenamento local de mensagens do usuário sem ter de buscar todo o conjunto de mensagens do usuário sempre que precisar dele.</span><span class="sxs-lookup"><span data-stu-id="ba410-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="ba410-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba410-108">Permissions</span></span>
<span data-ttu-id="ba410-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba410-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba410-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba410-111">Permission type</span></span>      | <span data-ttu-id="ba410-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba410-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba410-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba410-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ba410-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba410-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba410-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba410-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba410-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba410-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba410-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba410-117">Application</span></span> | <span data-ttu-id="ba410-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba410-118">Mail.ReadBasic.All , Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba410-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba410-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/{id}/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ba410-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="ba410-120">Query parameters</span></span>

<span data-ttu-id="ba410-p103">O controle de alterações em mensagens corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="ba410-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="ba410-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="ba410-126">Query parameter</span></span>      | <span data-ttu-id="ba410-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba410-127">Type</span></span>   |<span data-ttu-id="ba410-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba410-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba410-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ba410-129">$deltatoken</span></span> | <span data-ttu-id="ba410-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba410-130">string</span></span> | <span data-ttu-id="ba410-p104">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de mensagens indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="ba410-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="ba410-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ba410-133">$skiptoken</span></span> | <span data-ttu-id="ba410-134">string</span><span class="sxs-lookup"><span data-stu-id="ba410-134">string</span></span> | <span data-ttu-id="ba410-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ba410-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="ba410-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="ba410-136">OData query parameters</span></span>

- <span data-ttu-id="ba410-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="ba410-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="ba410-139">Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens.</span><span class="sxs-lookup"><span data-stu-id="ba410-139">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="ba410-140">Há suporte limitado para `$filter` e `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="ba410-140">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="ba410-141">As únicas expressões `$filter` suportadas são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="ba410-141">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="ba410-p106">A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.</span><span class="sxs-lookup"><span data-stu-id="ba410-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="ba410-144">Não há suporte para `$search`.</span><span class="sxs-lookup"><span data-stu-id="ba410-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba410-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba410-145">Request headers</span></span>
| <span data-ttu-id="ba410-146">Nome</span><span class="sxs-lookup"><span data-stu-id="ba410-146">Name</span></span>       | <span data-ttu-id="ba410-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba410-147">Type</span></span> | <span data-ttu-id="ba410-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba410-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="ba410-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba410-149">Authorization</span></span>  | <span data-ttu-id="ba410-150">string</span><span class="sxs-lookup"><span data-stu-id="ba410-150">string</span></span>  | <span data-ttu-id="ba410-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba410-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba410-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba410-153">Content-Type</span></span>  | <span data-ttu-id="ba410-154">string</span><span class="sxs-lookup"><span data-stu-id="ba410-154">string</span></span>  | <span data-ttu-id="ba410-p108">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba410-p108">application/json. Required.</span></span> |
| <span data-ttu-id="ba410-157">Preferir</span><span class="sxs-lookup"><span data-stu-id="ba410-157">Prefer</span></span> | <span data-ttu-id="ba410-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba410-158">string</span></span>  | <span data-ttu-id="ba410-p109">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ba410-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ba410-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba410-161">Response</span></span>

<span data-ttu-id="ba410-162">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba410-162">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba410-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba410-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba410-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba410-164">Request</span></span>
<span data-ttu-id="ba410-165">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de mensagens no corpo da resposta a dois.</span><span class="sxs-lookup"><span data-stu-id="ba410-165">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="ba410-p110">Para controlar alterações nas mensagens em uma pasta, faça uma ou mais chamadas de função **delta** para obter o conjunto de alterações incrementais desde a última consulta delta. Veja um exemplo que mostra uma série de chamadas de consulta delta em [Obter alterações incrementais para mensagens em uma pasta](/graph/delta-query-messages).</span><span class="sxs-lookup"><span data-stu-id="ba410-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 

# <a name="http"></a>[<span data-ttu-id="ba410-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba410-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="ba410-169">C#</span><span class="sxs-lookup"><span data-stu-id="ba410-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba410-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba410-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba410-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba410-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba410-172">Java</span><span class="sxs-lookup"><span data-stu-id="ba410-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba410-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba410-173">Response</span></span>
<span data-ttu-id="ba410-174">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="ba410-174">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="ba410-p111">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="ba410-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="ba410-177">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="ba410-177">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="ba410-p112">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba410-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/{id}/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="ba410-180">Confira também</span><span class="sxs-lookup"><span data-stu-id="ba410-180">See also</span></span>

- [<span data-ttu-id="ba410-181">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ba410-181">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ba410-182">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="ba410-182">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

