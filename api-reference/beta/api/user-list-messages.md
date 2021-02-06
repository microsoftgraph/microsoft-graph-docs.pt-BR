---
title: Listar mensagens
description: 'Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: e7eda13ab86c65ed2cfc8243a88d462a4348ee9c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130368"
---
# <a name="list-messages"></a><span data-ttu-id="ac6ae-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="ac6ae-103">List messages</span></span>

<span data-ttu-id="ac6ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6ae-105">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="ac6ae-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="ac6ae-106">Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="ac6ae-107">O tamanho de página padrão é 10 mensagens.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-107">The default page size is 10 messages.</span></span> <span data-ttu-id="ac6ae-108">Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="ac6ae-109">Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="ac6ae-110">Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="ac6ae-111">Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="ac6ae-112">Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="ac6ae-113">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="ac6ae-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="ac6ae-114">Você pode filtrar as mensagens e obter apenas aquelas que incluem uma [menção](../resources/mention.md) do usuário assinado.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-114">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="ac6ae-115">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-115">See an [example](#request-2) below.</span></span> <span data-ttu-id="ac6ae-116">Por padrão, a `GET /me/messages` operação não retorna a propriedade **menções.**</span><span class="sxs-lookup"><span data-stu-id="ac6ae-116">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="ac6ae-117">Use o `$expand` parâmetro de consulta para encontrar detalhes de cada [menção em uma mensagem.](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)</span><span class="sxs-lookup"><span data-stu-id="ac6ae-117">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).</span></span>

<span data-ttu-id="ac6ae-118">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-118">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="ac6ae-119">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="ac6ae-119">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ac6ae-120">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-120">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ac6ae-121">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="ac6ae-121">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="ac6ae-122">**Observação** Lembre-se da [questão conhecida](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) essa operação inclui mensagens de chat do Microsoft Teams em sua resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-122">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="ac6ae-123">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac6ae-123">Permissions</span></span>
<span data-ttu-id="ac6ae-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac6ae-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac6ae-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac6ae-126">Permission type</span></span>      | <span data-ttu-id="ac6ae-127">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac6ae-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac6ae-128">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac6ae-128">Delegated (work or school account)</span></span> | <span data-ttu-id="ac6ae-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac6ae-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ac6ae-130">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac6ae-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac6ae-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac6ae-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ac6ae-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac6ae-132">Application</span></span> | <span data-ttu-id="ac6ae-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac6ae-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac6ae-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6ae-134">HTTP request</span></span>

<span data-ttu-id="ac6ae-135">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-135">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="ac6ae-136">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-136">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="ac6ae-137">Para obter todas as mensagens na caixa de correio do usuário que incluem **uma menção** do usuário:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-137">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac6ae-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac6ae-138">Optional query parameters</span></span>
<span data-ttu-id="ac6ae-139">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="ac6ae-140">Você pode usar `$filter` o parâmetro de consulta na propriedade **mentionsPreview** para obter as mensagens que mencionam o usuário assinado.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-140">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="ac6ae-141">Uso de filtro e orderby na mesma consulta</span><span class="sxs-lookup"><span data-stu-id="ac6ae-141">Using filter and orderby in the same query</span></span>
<span data-ttu-id="ac6ae-142">Ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens, lembre-se de especificar as propriedades das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-142">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="ac6ae-143">As propriedades que aparecem em `$orderby` também devem aparecer em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-143">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="ac6ae-144">As propriedades que aparecem em `$orderby` estão na mesma ordem que em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-144">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="ac6ae-145">As propriedades presentes em `$orderby` aparecem em `$filter` antes de qualquer propriedade que não esteja presente.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-145">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="ac6ae-146">Ao não fazer isso, o seguinte erro surge:</span><span class="sxs-lookup"><span data-stu-id="ac6ae-146">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="ac6ae-147">Código de erro: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="ac6ae-147">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="ac6ae-148">Mensagem de erro: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="ac6ae-148">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac6ae-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac6ae-149">Request headers</span></span>
| <span data-ttu-id="ac6ae-150">Nome</span><span class="sxs-lookup"><span data-stu-id="ac6ae-150">Name</span></span>       | <span data-ttu-id="ac6ae-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac6ae-151">Type</span></span> | <span data-ttu-id="ac6ae-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6ae-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ac6ae-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac6ae-153">Authorization</span></span>  | <span data-ttu-id="ac6ae-154">string</span><span class="sxs-lookup"><span data-stu-id="ac6ae-154">string</span></span>  | <span data-ttu-id="ac6ae-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac6ae-157">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ac6ae-157">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ac6ae-158">string</span><span class="sxs-lookup"><span data-stu-id="ac6ae-158">string</span></span> | <span data-ttu-id="ac6ae-159">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-159">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="ac6ae-160">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="ac6ae-160">Values can be "text" or "html".</span></span> <span data-ttu-id="ac6ae-161">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-161">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="ac6ae-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-162">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac6ae-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac6ae-163">Request body</span></span>
<span data-ttu-id="ac6ae-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac6ae-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac6ae-165">Response</span></span>

<span data-ttu-id="ac6ae-166">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de objetos [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-166">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac6ae-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac6ae-167">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ac6ae-168">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="ac6ae-168">Request 1</span></span>
<span data-ttu-id="ac6ae-169">O primeiro exemplo obtém as 10 principais mensagens padrão na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-169">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="ac6ae-170">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-170">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="ac6ae-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6ae-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="ac6ae-172">C#</span><span class="sxs-lookup"><span data-stu-id="ac6ae-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac6ae-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6ae-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac6ae-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6ae-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac6ae-175">Java</span><span class="sxs-lookup"><span data-stu-id="ac6ae-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="ac6ae-176">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="ac6ae-176">Response 1</span></span>
<span data-ttu-id="ac6ae-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-177">Here is an example of the response.</span></span> <span data-ttu-id="ac6ae-178">Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-178">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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


##### <a name="request-2"></a><span data-ttu-id="ac6ae-179">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="ac6ae-179">Request 2</span></span>
<span data-ttu-id="ac6ae-180">O próximo exemplo filtra todas as mensagens na caixa de correio do usuário que o mencionam.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-180">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="ac6ae-181">Ele também usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-181">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="ac6ae-182">O exemplo também incorpora a codificação de URL para os caracteres de espaço na cadeia de caracteres do parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-182">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac6ae-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6ae-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="ac6ae-184">C#</span><span class="sxs-lookup"><span data-stu-id="ac6ae-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac6ae-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6ae-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac6ae-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6ae-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac6ae-187">Java</span><span class="sxs-lookup"><span data-stu-id="ac6ae-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="ac6ae-188">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="ac6ae-188">Response 2</span></span>
<span data-ttu-id="ac6ae-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="ac6ae-192">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="ac6ae-192">Request 3</span></span>
<span data-ttu-id="ac6ae-193">O terceiro exemplo mostra como usar um header para obter o corpo e as propriedades `Prefer: outlook.body-content-type="text"` **uniqueBody** de cada mensagem no formato de texto. </span><span class="sxs-lookup"><span data-stu-id="ac6ae-193">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac6ae-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6ae-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="ac6ae-195">C#</span><span class="sxs-lookup"><span data-stu-id="ac6ae-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac6ae-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6ae-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac6ae-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6ae-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac6ae-198">Java</span><span class="sxs-lookup"><span data-stu-id="ac6ae-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="ac6ae-199">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="ac6ae-199">Response 3</span></span>
<span data-ttu-id="ac6ae-200">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac6ae-200">Here is an example of the response.</span></span> 

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
