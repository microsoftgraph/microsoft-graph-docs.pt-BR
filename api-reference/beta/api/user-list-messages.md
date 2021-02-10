---
title: Listar mensagens
description: 'Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 87a5fc5f29d23b6c9a7fbbe48b059066001d5419
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176988"
---
# <a name="list-messages"></a><span data-ttu-id="e845d-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="e845d-103">List messages</span></span>

<span data-ttu-id="e845d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e845d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e845d-105">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="e845d-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="e845d-106">Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="e845d-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="e845d-107">O tamanho de página padrão é 10 mensagens.</span><span class="sxs-lookup"><span data-stu-id="e845d-107">The default page size is 10 messages.</span></span> <span data-ttu-id="e845d-108">Use `$top` para personalizar o tamanho da página, dentro do intervalo de 1 e 1000.</span><span class="sxs-lookup"><span data-stu-id="e845d-108">Use `$top` to customize the page size, within the range of 1 and 1000.</span></span>

<span data-ttu-id="e845d-109">Para melhorar o tempo de resposta da operação, use para especificar as propriedades exatas de que você `$select` precisa; consulte [o exemplo 1](#example-1-list-all-messages) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e845d-109">To improve the operation response time, use `$select` to specify the exact properties you need; see [example 1](#example-1-list-all-messages) below.</span></span> <span data-ttu-id="e845d-110">Ajuste os valores para e, especialmente quando você deve usar um tamanho de página maior, pois retornar uma página com centenas de mensagens cada uma com uma carga de resposta completa pode disparar o tempo de vida do `$select` `$top` [gateway](/graph/errors#http-status-codes) (HTTP 504).</span><span class="sxs-lookup"><span data-stu-id="e845d-110">Fine-tune the values for `$select` and `$top`, especially when you must use a larger page size, as returning a page with hundreds of messages each with a full response payload may trigger the [gateway timeout](/graph/errors#http-status-codes) (HTTP 504).</span></span>

<span data-ttu-id="e845d-111">Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="e845d-111">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="e845d-112">Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="e845d-112">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="e845d-113">Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas.</span><span class="sxs-lookup"><span data-stu-id="e845d-113">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="e845d-114">Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem.</span><span class="sxs-lookup"><span data-stu-id="e845d-114">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="e845d-115">Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="e845d-115">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="e845d-116">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="e845d-116">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="e845d-117">Você pode filtrar as mensagens e obter apenas aquelas que incluem [uma](../resources/mention.md) menção do usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="e845d-117">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="e845d-118">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e845d-118">See an [example](#request-2) below.</span></span> <span data-ttu-id="e845d-119">Por padrão, a `GET /me/messages` operação não retorna a propriedade **menções.**</span><span class="sxs-lookup"><span data-stu-id="e845d-119">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="e845d-120">Use o `$expand` parâmetro de consulta para encontrar detalhes de cada [menção em uma mensagem.](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)</span><span class="sxs-lookup"><span data-stu-id="e845d-120">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).</span></span>

<span data-ttu-id="e845d-121">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="e845d-121">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="e845d-122">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="e845d-122">If the app has application permissions, or,</span></span>
* <span data-ttu-id="e845d-123">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="e845d-123">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="e845d-124">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="e845d-124">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="e845d-125">**Observação** Lembre-se da [questão conhecida](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) essa operação inclui mensagens de chat do Microsoft Teams em sua resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-125">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="e845d-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="e845d-126">Permissions</span></span>
<span data-ttu-id="e845d-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e845d-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e845d-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e845d-129">Permission type</span></span>      | <span data-ttu-id="e845d-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e845d-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e845d-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e845d-131">Delegated (work or school account)</span></span> | <span data-ttu-id="e845d-132">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e845d-132">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e845d-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e845d-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e845d-134">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e845d-134">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e845d-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e845d-135">Application</span></span> | <span data-ttu-id="e845d-136">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e845d-136">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e845d-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e845d-137">HTTP request</span></span>

<span data-ttu-id="e845d-138">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="e845d-138">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="e845d-139">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="e845d-139">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="e845d-140">Para obter todas as mensagens na caixa de correio do usuário que incluem **uma menção** do usuário:</span><span class="sxs-lookup"><span data-stu-id="e845d-140">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e845d-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e845d-141">Optional query parameters</span></span>
<span data-ttu-id="e845d-142">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="e845d-143">Você pode usar `$filter` o parâmetro de consulta na propriedade **mentionsPreview** para obter as mensagens que mencionam o usuário assinado.</span><span class="sxs-lookup"><span data-stu-id="e845d-143">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="e845d-144">Uso de filtro e orderby na mesma consulta</span><span class="sxs-lookup"><span data-stu-id="e845d-144">Using filter and orderby in the same query</span></span>
<span data-ttu-id="e845d-145">Ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens, lembre-se de especificar as propriedades das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e845d-145">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="e845d-146">As propriedades que aparecem em `$orderby` também devem aparecer em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e845d-146">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="e845d-147">As propriedades que aparecem em `$orderby` estão na mesma ordem que em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e845d-147">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="e845d-148">As propriedades presentes em `$orderby` aparecem em `$filter` antes de qualquer propriedade que não esteja presente.</span><span class="sxs-lookup"><span data-stu-id="e845d-148">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="e845d-149">Ao não fazer isso, o seguinte erro surge:</span><span class="sxs-lookup"><span data-stu-id="e845d-149">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="e845d-150">Código de erro: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="e845d-150">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="e845d-151">Mensagem de erro: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="e845d-151">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="e845d-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e845d-152">Request headers</span></span>
| <span data-ttu-id="e845d-153">Nome</span><span class="sxs-lookup"><span data-stu-id="e845d-153">Name</span></span>       | <span data-ttu-id="e845d-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="e845d-154">Type</span></span> | <span data-ttu-id="e845d-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="e845d-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e845d-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="e845d-156">Authorization</span></span>  | <span data-ttu-id="e845d-157">string</span><span class="sxs-lookup"><span data-stu-id="e845d-157">string</span></span>  | <span data-ttu-id="e845d-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e845d-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e845d-160">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e845d-160">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e845d-161">string</span><span class="sxs-lookup"><span data-stu-id="e845d-161">string</span></span> | <span data-ttu-id="e845d-162">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="e845d-162">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="e845d-163">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="e845d-163">Values can be "text" or "html".</span></span> <span data-ttu-id="e845d-164">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="e845d-164">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="e845d-165">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e845d-165">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e845d-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e845d-166">Request body</span></span>
<span data-ttu-id="e845d-167">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e845d-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e845d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e845d-168">Response</span></span>

<span data-ttu-id="e845d-169">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de objetos [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-169">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e845d-170">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e845d-170">Examples</span></span>
### <a name="example-1-list-all-messages"></a><span data-ttu-id="e845d-171">Exemplo 1: Listar todas as mensagens</span><span class="sxs-lookup"><span data-stu-id="e845d-171">Example 1: List all messages</span></span>
#### <a name="request"></a><span data-ttu-id="e845d-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e845d-172">Request</span></span>
<span data-ttu-id="e845d-173">O primeiro exemplo obtém as 10 principais mensagens padrão na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e845d-173">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="e845d-174">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-174">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="e845d-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="e845d-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="e845d-176">C#</span><span class="sxs-lookup"><span data-stu-id="e845d-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e845d-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e845d-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e845d-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e845d-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e845d-179">Java</span><span class="sxs-lookup"><span data-stu-id="e845d-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e845d-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="e845d-180">Response</span></span>
<span data-ttu-id="e845d-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-181">Here is an example of the response.</span></span> <span data-ttu-id="e845d-182">Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.</span><span class="sxs-lookup"><span data-stu-id="e845d-182">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
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
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        }
    ]
}
```

### <a name="example-2-use-filter-to-get-all-messages-satisfying-a-specific-condition"></a><span data-ttu-id="e845d-183">Exemplo 2: Use $filter para obter todas as mensagens que satisfazem uma condição específica</span><span class="sxs-lookup"><span data-stu-id="e845d-183">Example 2: Use $filter to get all messages satisfying a specific condition</span></span>
#### <a name="request"></a><span data-ttu-id="e845d-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e845d-184">Request</span></span>
<span data-ttu-id="e845d-185">O próximo exemplo filtra todas as mensagens na caixa de correio do usuário que o mencionam.</span><span class="sxs-lookup"><span data-stu-id="e845d-185">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="e845d-186">Ele também usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-186">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="e845d-187">O exemplo também incorpora a codificação de URL para os caracteres de espaço na cadeia de caracteres do parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="e845d-187">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="e845d-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="e845d-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="e845d-189">C#</span><span class="sxs-lookup"><span data-stu-id="e845d-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e845d-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e845d-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e845d-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e845d-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e845d-192">Java</span><span class="sxs-lookup"><span data-stu-id="e845d-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e845d-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="e845d-193">Response</span></span>
<span data-ttu-id="e845d-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e845d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

### <a name="example-3-use-prefer-header-to-get-the-message-body-and-uniquebody-is-text-format"></a><span data-ttu-id="e845d-197">Exemplo 3: Usar o header prefer para obter o corpo da mensagem e uniqueBody é o formato de texto</span><span class="sxs-lookup"><span data-stu-id="e845d-197">Example 3: Use prefer header to get the message body and uniqueBody is text format</span></span>
#### <a name="request"></a><span data-ttu-id="e845d-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e845d-198">Request</span></span>
<span data-ttu-id="e845d-199">O terceiro exemplo mostra como usar um header para obter o corpo e as propriedades `Prefer: outlook.body-content-type="text"` **uniqueBody** de cada mensagem no formato de texto. </span><span class="sxs-lookup"><span data-stu-id="e845d-199">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="e845d-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="e845d-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="e845d-201">C#</span><span class="sxs-lookup"><span data-stu-id="e845d-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e845d-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e845d-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e845d-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e845d-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e845d-204">Java</span><span class="sxs-lookup"><span data-stu-id="e845d-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e845d-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="e845d-205">Response</span></span>
<span data-ttu-id="e845d-206">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e845d-206">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
