---
title: Listar mensagens
description: Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6086c3acf463e5fe4ffc130af3d9b95435061ba
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982975"
---
# <a name="list-messages"></a><span data-ttu-id="66748-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="66748-103">List messages</span></span>

<span data-ttu-id="66748-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66748-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66748-105">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="66748-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="66748-106">Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="66748-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="66748-107">O tamanho de página padrão é 10 mensagens.</span><span class="sxs-lookup"><span data-stu-id="66748-107">The default page size is 10 messages.</span></span> <span data-ttu-id="66748-108">Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="66748-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="66748-109">Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="66748-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="66748-110">Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas.</span><span class="sxs-lookup"><span data-stu-id="66748-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="66748-111">Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem.</span><span class="sxs-lookup"><span data-stu-id="66748-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="66748-112">Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="66748-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="66748-113">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="66748-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="66748-114">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="66748-114">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="66748-115">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="66748-115">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="66748-116">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="66748-116">If the app has application permissions, or,</span></span>
* <span data-ttu-id="66748-117">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="66748-117">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="66748-118">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="66748-118">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="66748-119">**Observação** Lembre-se da [questão conhecida](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) essa operação inclui mensagens de chat do Microsoft Teams em sua resposta.</span><span class="sxs-lookup"><span data-stu-id="66748-119">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>

## <a name="permissions"></a><span data-ttu-id="66748-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="66748-120">Permissions</span></span>
<span data-ttu-id="66748-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66748-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66748-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66748-123">Permission type</span></span>      | <span data-ttu-id="66748-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66748-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66748-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66748-125">Delegated (work or school account)</span></span> | <span data-ttu-id="66748-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66748-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="66748-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66748-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66748-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66748-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="66748-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66748-129">Application</span></span> | <span data-ttu-id="66748-130">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66748-130">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66748-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66748-131">HTTP request</span></span>

<span data-ttu-id="66748-132">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="66748-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="66748-133">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="66748-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66748-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66748-134">Optional query parameters</span></span>
<span data-ttu-id="66748-135">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66748-135">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="66748-136">Uso de filtro e orderby na mesma consulta</span><span class="sxs-lookup"><span data-stu-id="66748-136">Using filter and orderby in the same query</span></span>
<span data-ttu-id="66748-137">Ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens, lembre-se de especificar as propriedades das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="66748-137">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="66748-138">As propriedades que aparecem em `$orderby` também devem aparecer em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="66748-138">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="66748-139">As propriedades que aparecem em `$orderby` estão na mesma ordem que em `$filter`.</span><span class="sxs-lookup"><span data-stu-id="66748-139">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="66748-140">As propriedades presentes em `$orderby` aparecem em `$filter` antes de qualquer propriedade que não esteja presente.</span><span class="sxs-lookup"><span data-stu-id="66748-140">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="66748-141">Ao não fazer isso, o seguinte erro surge:</span><span class="sxs-lookup"><span data-stu-id="66748-141">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="66748-142">Código de erro: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="66748-142">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="66748-143">Mensagem de erro: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="66748-143">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="66748-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66748-144">Request headers</span></span>
| <span data-ttu-id="66748-145">Nome</span><span class="sxs-lookup"><span data-stu-id="66748-145">Name</span></span>       | <span data-ttu-id="66748-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="66748-146">Type</span></span> | <span data-ttu-id="66748-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="66748-147">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66748-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="66748-148">Authorization</span></span>  | <span data-ttu-id="66748-149">string</span><span class="sxs-lookup"><span data-stu-id="66748-149">string</span></span>  | <span data-ttu-id="66748-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66748-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66748-152">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="66748-152">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="66748-153">string</span><span class="sxs-lookup"><span data-stu-id="66748-153">string</span></span> | <span data-ttu-id="66748-154">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="66748-154">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="66748-155">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="66748-155">Values can be "text" or "html".</span></span> <span data-ttu-id="66748-156">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="66748-156">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="66748-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="66748-157">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="66748-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66748-158">Request body</span></span>
<span data-ttu-id="66748-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66748-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66748-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="66748-160">Response</span></span>

<span data-ttu-id="66748-161">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66748-161">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66748-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66748-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66748-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66748-163">Request</span></span>
<span data-ttu-id="66748-164">Este exemplo obtém as 10 mensagens principais padrão na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="66748-164">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="66748-165">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="66748-165">It uses `$select` to return a subset of the properties of each message in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="66748-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="66748-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="66748-167">C#</span><span class="sxs-lookup"><span data-stu-id="66748-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66748-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66748-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66748-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66748-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66748-170">Java</span><span class="sxs-lookup"><span data-stu-id="66748-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66748-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="66748-171">Response</span></span>
<span data-ttu-id="66748-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66748-172">Here is an example of the response.</span></span> <span data-ttu-id="66748-173">Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.</span><span class="sxs-lookup"><span data-stu-id="66748-173">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$select=sender%2csubject&$skip=14",
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
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dft\"",
            "id": "AAMkAGUAAAq5UMVAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DfF\"",
            "id": "AAMkAGUAAAq5UMUAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
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
