---
title: Listar mensagens
description: 'Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). '
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3c6cb96d60554c3e2a2dd0d012e5069bae6b1f78
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422118"
---
# <a name="list-messages"></a><span data-ttu-id="00405-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="00405-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00405-104">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="00405-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="00405-105">Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="00405-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="00405-106">O tamanho de página padrão é 10 mensagens.</span><span class="sxs-lookup"><span data-stu-id="00405-106">The default page size is 10 messages.</span></span> <span data-ttu-id="00405-107">Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="00405-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="00405-108">Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="00405-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="00405-109">Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas.</span><span class="sxs-lookup"><span data-stu-id="00405-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="00405-110">Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem.</span><span class="sxs-lookup"><span data-stu-id="00405-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="00405-111">Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="00405-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="00405-112">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="00405-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="00405-113">Você pode filtrar as mensagens e obter apenas aquelas que incluem [menção](../resources/mention.md) do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="00405-113">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="00405-114">Observe que, por padrão, `GET /me/messages` a operação não retorna a propriedade **menciona** .</span><span class="sxs-lookup"><span data-stu-id="00405-114">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="00405-115">Use o `$expand` parâmetro de consulta para [encontrar detalhes de cada menção em uma mensagem](../api/message-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="00405-115">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="00405-116">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="00405-116">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="00405-117">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="00405-117">If the app has application permissions, or,</span></span>
* <span data-ttu-id="00405-118">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="00405-118">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="00405-119">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="00405-119">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="00405-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="00405-120">Permissions</span></span>
<span data-ttu-id="00405-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00405-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00405-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00405-123">Permission type</span></span>      | <span data-ttu-id="00405-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00405-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00405-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00405-125">Delegated (work or school account)</span></span> | <span data-ttu-id="00405-126">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00405-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00405-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00405-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00405-128">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00405-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00405-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00405-129">Application</span></span> | <span data-ttu-id="00405-130">Mail. ReadBasic. All, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00405-130">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00405-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00405-131">HTTP request</span></span>

<span data-ttu-id="00405-132">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="00405-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="00405-133">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="00405-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="00405-134">Para obter todas as mensagens na caixa de correio do usuário que incluam um **menção** do usuário:</span><span class="sxs-lookup"><span data-stu-id="00405-134">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00405-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00405-135">Optional query parameters</span></span>
<span data-ttu-id="00405-136">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="00405-137">Você pode usar o `$filter` parâmetro de consulta na propriedade **mentionsPreview** para obter as mensagens que mencionam o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="00405-137">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00405-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00405-138">Request headers</span></span>
| <span data-ttu-id="00405-139">Nome</span><span class="sxs-lookup"><span data-stu-id="00405-139">Name</span></span>       | <span data-ttu-id="00405-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="00405-140">Type</span></span> | <span data-ttu-id="00405-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="00405-141">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="00405-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="00405-142">Authorization</span></span>  | <span data-ttu-id="00405-143">string</span><span class="sxs-lookup"><span data-stu-id="00405-143">string</span></span>  | <span data-ttu-id="00405-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00405-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00405-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="00405-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="00405-147">string</span><span class="sxs-lookup"><span data-stu-id="00405-147">string</span></span> | <span data-ttu-id="00405-148">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="00405-148">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="00405-149">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="00405-149">Values can be "text" or "html".</span></span> <span data-ttu-id="00405-150">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="00405-150">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="00405-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="00405-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00405-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00405-152">Request body</span></span>
<span data-ttu-id="00405-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00405-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00405-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="00405-154">Response</span></span>

<span data-ttu-id="00405-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-155">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00405-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00405-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="00405-157">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="00405-157">Request 1</span></span>
<span data-ttu-id="00405-158">O primeiro exemplo obtém o padrão, as 10 principais mensagens na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="00405-158">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="00405-159">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-159">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="00405-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="00405-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00405-161">C#</span><span class="sxs-lookup"><span data-stu-id="00405-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00405-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00405-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00405-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00405-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="00405-164">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="00405-164">Response 1</span></span>
<span data-ttu-id="00405-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-165">Here is an example of the response.</span></span> <span data-ttu-id="00405-166">Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.</span><span class="sxs-lookup"><span data-stu-id="00405-166">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
                    "address": "azure-noreply@microsoft.com"
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
                    "address": "MeganB@contoso.OnMicrosoft.com"
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
                    "address": "MeganB@contoso.OnMicrosoft.com"
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
                    "address": "MeganB@contoso.OnMicrosoft.com"
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
                    "address": "MeganB@contoso.OnMicrosoft.com"
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
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="00405-167">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="00405-167">Request 2</span></span>
<span data-ttu-id="00405-168">O próximo exemplo filtra todas as mensagens na caixa de correio do usuário conectado para as que mencionam o usuário.</span><span class="sxs-lookup"><span data-stu-id="00405-168">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="00405-169">Ele também usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-169">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="00405-170">O exemplo também incorpora a codificação de URL para os caracteres de espaço na cadeia de caracteres de parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="00405-170">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00405-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="00405-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00405-172">C#</span><span class="sxs-lookup"><span data-stu-id="00405-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00405-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00405-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00405-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00405-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="00405-175">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="00405-175">Response 2</span></span>
<span data-ttu-id="00405-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00405-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
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
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="00405-179">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="00405-179">Request 3</span></span>
<span data-ttu-id="00405-180">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter as propriedades **Body** e **uniqueBody** de cada mensagem em formato de texto.</span><span class="sxs-lookup"><span data-stu-id="00405-180">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00405-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="00405-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00405-182">C#</span><span class="sxs-lookup"><span data-stu-id="00405-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00405-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00405-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00405-184">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00405-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="00405-185">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="00405-185">Response 3</span></span>
<span data-ttu-id="00405-186">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00405-186">Here is an example of the response.</span></span> 

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
