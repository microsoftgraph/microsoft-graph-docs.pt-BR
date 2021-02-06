---
title: 'mailFolder: delta'
description: Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f0105e2da5c625e99250d3f6c2e4d383090a6be3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128483"
---
# <a name="mailfolder-delta"></a><span data-ttu-id="91fd9-103">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="91fd9-103">mailFolder: delta</span></span>

<span data-ttu-id="91fd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91fd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91fd9-105">Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="91fd9-105">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="91fd9-p101">Uma chamada de função **delta** de pastas de email em uma caixa de correio é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite consultar alterações incrementais nas pastas de email. Isso permite manter e sincronizar um armazenamento local de pastas de email do usuário sem ter que sempre buscar todas as pastas de email dessa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="91fd9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="91fd9-108">Permissions</span></span>
<span data-ttu-id="91fd9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91fd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="91fd9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91fd9-111">Permission type</span></span>      | <span data-ttu-id="91fd9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91fd9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91fd9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91fd9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91fd9-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91fd9-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91fd9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91fd9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91fd9-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91fd9-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91fd9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91fd9-117">Application</span></span> | <span data-ttu-id="91fd9-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91fd9-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91fd9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91fd9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="91fd9-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="91fd9-120">Query parameters</span></span>

<span data-ttu-id="91fd9-p103">O controle de alterações em pastas de email corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="91fd9-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="91fd9-126">Query parameter</span></span>      | <span data-ttu-id="91fd9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="91fd9-127">Type</span></span>   |<span data-ttu-id="91fd9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="91fd9-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91fd9-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="91fd9-129">$deltatoken</span></span> | <span data-ttu-id="91fd9-130">string</span><span class="sxs-lookup"><span data-stu-id="91fd9-130">string</span></span> | <span data-ttu-id="91fd9-p104">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de pastas de email indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="91fd9-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="91fd9-133">$skiptoken</span></span> | <span data-ttu-id="91fd9-134">string</span><span class="sxs-lookup"><span data-stu-id="91fd9-134">string</span></span> | <span data-ttu-id="91fd9-135">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de pastas de email.</span><span class="sxs-lookup"><span data-stu-id="91fd9-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="91fd9-136">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="91fd9-136">OData query parameters</span></span>

<span data-ttu-id="91fd9-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="91fd9-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91fd9-139">Request headers</span></span>
| <span data-ttu-id="91fd9-140">Nome</span><span class="sxs-lookup"><span data-stu-id="91fd9-140">Name</span></span>       | <span data-ttu-id="91fd9-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="91fd9-141">Type</span></span> | <span data-ttu-id="91fd9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="91fd9-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="91fd9-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="91fd9-143">Authorization</span></span>  | <span data-ttu-id="91fd9-144">string</span><span class="sxs-lookup"><span data-stu-id="91fd9-144">string</span></span>  | <span data-ttu-id="91fd9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91fd9-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91fd9-147">Content-Type</span></span>  | <span data-ttu-id="91fd9-148">string</span><span class="sxs-lookup"><span data-stu-id="91fd9-148">string</span></span>  | <span data-ttu-id="91fd9-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p107">application/json. Required.</span></span> |
| <span data-ttu-id="91fd9-151">Preferir</span><span class="sxs-lookup"><span data-stu-id="91fd9-151">Prefer</span></span> | <span data-ttu-id="91fd9-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91fd9-152">string</span></span>  | <span data-ttu-id="91fd9-p108">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="91fd9-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fd9-155">Response</span></span>

<span data-ttu-id="91fd9-156">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91fd9-156">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91fd9-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91fd9-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91fd9-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91fd9-158">Request</span></span>
<span data-ttu-id="91fd9-159">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de pastas de email no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="91fd9-159">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="91fd9-160">Para controlar as alterações nas pastas de email de uma caixa de correio, faça uma ou mais chamadas de função **delta**, com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="91fd9-160">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="91fd9-p109">Você pode encontrar um exemplo semelhante que mostra como usar os tokens de estado para controlar alterações em mensagens de uma pasta de email: [Obtenha alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages). As principais diferenças entre o controle de pastas de email e o controle de mensagens em uma pasta encontram-se nas URLs das solicitações da consulta delta e nas respostas da consulta que retornam **mailFolder** em vez de coleções de **mensagens**.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>


# <a name="http"></a>[<span data-ttu-id="91fd9-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="91fd9-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="91fd9-164">C#</span><span class="sxs-lookup"><span data-stu-id="91fd9-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91fd9-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91fd9-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91fd9-166">Java</span><span class="sxs-lookup"><span data-stu-id="91fd9-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91fd9-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fd9-167">Response</span></span>

<span data-ttu-id="91fd9-168">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="91fd9-168">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="91fd9-p110">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="91fd9-171">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="91fd9-171">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="91fd9-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91fd9-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="91fd9-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="91fd9-174">See also</span></span>

- [<span data-ttu-id="91fd9-175">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="91fd9-175">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="91fd9-176">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="91fd9-176">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


