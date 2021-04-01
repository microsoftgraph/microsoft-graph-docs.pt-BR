---
title: Listar mensagens
description: Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ad594f12603668d0684523a25cd708be8b61eae8
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473959"
---
# <a name="list-messages"></a><span data-ttu-id="5f709-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="5f709-103">List messages</span></span>

<span data-ttu-id="5f709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f709-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f709-105">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="5f709-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="5f709-106">Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="5f709-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="5f709-107">O tamanho de página padrão é 10 mensagens.</span><span class="sxs-lookup"><span data-stu-id="5f709-107">The default page size is 10 messages.</span></span> <span data-ttu-id="5f709-108">Use `$top` para personalizar o tamanho da página, no intervalo de 1 a 1000.</span><span class="sxs-lookup"><span data-stu-id="5f709-108">Use `$top` to customize the page size, within the range of 1 and 1000.</span></span>

<span data-ttu-id="5f709-109">Para melhorar o tempo de resposta da operação, use `$select` para especificar as propriedades exatas de que você precisa; consulte [exemplo 1](#example-1-list-all-messages) abaixo.</span><span class="sxs-lookup"><span data-stu-id="5f709-109">To improve the operation response time, use `$select` to specify the exact properties you need; see [example 1](#example-1-list-all-messages) below.</span></span> <span data-ttu-id="5f709-110">Ajuste os valores para `$select` e `$top`, especialmente quando você deve usar um tamanho de página maior, pois retornar uma página com centenas de mensagens, cada uma com uma carga útil de resposta completa, pode acionar o [tempo limite do gateway](/graph/errors#http-status-codes) (HTTP 504).</span><span class="sxs-lookup"><span data-stu-id="5f709-110">Fine-tune the values for `$select` and `$top`, especially when you must use a larger page size, as returning a page with hundreds of messages each with a full response payload may trigger the [gateway timeout](/graph/errors#http-status-codes) (HTTP 504).</span></span>

<span data-ttu-id="5f709-111">Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="5f709-111">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="5f709-112">Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="5f709-112">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="5f709-113">Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas.</span><span class="sxs-lookup"><span data-stu-id="5f709-113">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="5f709-114">Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem.</span><span class="sxs-lookup"><span data-stu-id="5f709-114">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="5f709-115">Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="5f709-115">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="5f709-116">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="5f709-116">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="5f709-117">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5f709-117">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="5f709-118">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="5f709-118">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="5f709-119">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="5f709-119">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5f709-120">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5f709-120">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5f709-121">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="5f709-121">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="5f709-122">**Observação** Lembre-se da [questão conhecida](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) essa operação inclui mensagens de chat do Microsoft Teams em sua resposta.</span><span class="sxs-lookup"><span data-stu-id="5f709-122">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f709-123">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f709-123">Permissions</span></span>
<span data-ttu-id="5f709-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f709-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f709-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f709-126">Permission type</span></span>      | <span data-ttu-id="5f709-127">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f709-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f709-128">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f709-128">Delegated (work or school account)</span></span> | <span data-ttu-id="5f709-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f709-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f709-130">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f709-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f709-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f709-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f709-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f709-132">Application</span></span> | <span data-ttu-id="5f709-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f709-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f709-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f709-134">HTTP request</span></span>

<span data-ttu-id="5f709-135">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="5f709-135">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="5f709-136">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="5f709-136">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f709-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f709-137">Optional query parameters</span></span>
<span data-ttu-id="5f709-138">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f709-138">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="5f709-139">Uso de filtro e orderby na mesma consulta</span><span class="sxs-lookup"><span data-stu-id="5f709-139">Using filter and orderby in the same query</span></span>
<span data-ttu-id="5f709-140">Ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens, lembre-se de especificar as propriedades das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="5f709-140">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="5f709-141">As propriedades que aparecem em `$orderby` também devem aparecer em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5f709-141">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="5f709-142">As propriedades que aparecem em `$orderby` estão na mesma ordem que em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5f709-142">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="5f709-143">As propriedades presentes em `$orderby` aparecem em `$filter` antes de qualquer propriedade que não esteja presente.</span><span class="sxs-lookup"><span data-stu-id="5f709-143">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="5f709-144">Ao não fazer isso, o seguinte erro surge:</span><span class="sxs-lookup"><span data-stu-id="5f709-144">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="5f709-145">Código de erro: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="5f709-145">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="5f709-146">Mensagem de erro: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="5f709-146">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f709-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f709-147">Request headers</span></span>
| <span data-ttu-id="5f709-148">Nome</span><span class="sxs-lookup"><span data-stu-id="5f709-148">Name</span></span>       | <span data-ttu-id="5f709-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f709-149">Type</span></span> | <span data-ttu-id="5f709-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f709-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5f709-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f709-151">Authorization</span></span>  | <span data-ttu-id="5f709-152">string</span><span class="sxs-lookup"><span data-stu-id="5f709-152">string</span></span>  | <span data-ttu-id="5f709-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f709-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f709-155">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5f709-155">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5f709-156">string</span><span class="sxs-lookup"><span data-stu-id="5f709-156">string</span></span> | <span data-ttu-id="5f709-157">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="5f709-157">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="5f709-158">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="5f709-158">Values can be "text" or "html".</span></span> <span data-ttu-id="5f709-159">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5f709-159">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="5f709-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5f709-160">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5f709-161">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f709-161">Request body</span></span>
<span data-ttu-id="5f709-162">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f709-162">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f709-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f709-163">Response</span></span>

<span data-ttu-id="5f709-164">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f709-164">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f709-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f709-165">Examples</span></span>
### <a name="example-1-list-all-messages"></a><span data-ttu-id="5f709-166">Exemplo 1: Listar todas as mensagens</span><span class="sxs-lookup"><span data-stu-id="5f709-166">Example 1: List all messages</span></span>
#### <a name="request"></a><span data-ttu-id="5f709-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f709-167">Request</span></span>
<span data-ttu-id="5f709-168">Este exemplo obtém as 10 mensagens principais padrão na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5f709-168">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="5f709-169">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f709-169">It uses `$select` to return a subset of the properties of each message in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f709-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f709-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="5f709-171">C#</span><span class="sxs-lookup"><span data-stu-id="5f709-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f709-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f709-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f709-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f709-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f709-174">Java</span><span class="sxs-lookup"><span data-stu-id="5f709-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5f709-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f709-175">Response</span></span>
<span data-ttu-id="5f709-176">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f709-176">Here is an example of the response.</span></span> <span data-ttu-id="5f709-177">Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.</span><span class="sxs-lookup"><span data-stu-id="5f709-177">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "value": [
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
            "id": "AAMkAGUAAAwTW09AAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
