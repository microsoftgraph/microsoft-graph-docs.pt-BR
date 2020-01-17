---
title: Obter mensagem
description: Recupere as propriedades e os relacionamentos de um objeto message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cc45adb31d22502878cc7c8cad2c9d85eed3f91e
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216879"
---
# <a name="get-message"></a><span data-ttu-id="6dcbd-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="6dcbd-103">Get message</span></span>

<span data-ttu-id="6dcbd-104">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6dcbd-105">Você pode usar o `$value` parâmetro para [obter o conteúdo MIME de uma mensagem](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-105">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="6dcbd-106">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="6dcbd-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="6dcbd-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="6dcbd-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6dcbd-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6dcbd-109">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="6dcbd-110">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="6dcbd-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dcbd-111">Permissions</span></span>
<span data-ttu-id="6dcbd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dcbd-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dcbd-114">Permission type</span></span>      | <span data-ttu-id="6dcbd-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dcbd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dcbd-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dcbd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6dcbd-117">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6dcbd-117">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="6dcbd-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dcbd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dcbd-119">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6dcbd-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="6dcbd-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dcbd-120">Application</span></span> | <span data-ttu-id="6dcbd-121">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6dcbd-121">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dcbd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dcbd-122">HTTP request</span></span>

<span data-ttu-id="6dcbd-123">Para obter a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="6dcbd-123">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="6dcbd-124">Para obter o conteúdo MIME da mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="6dcbd-124">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dcbd-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6dcbd-125">Optional query parameters</span></span>
<span data-ttu-id="6dcbd-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6dcbd-127">Use o parâmetro `$value` para obter o conteúdo MIME de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-127">Use the `$value` parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6dcbd-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-128">Request headers</span></span>
| <span data-ttu-id="6dcbd-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6dcbd-129">Name</span></span>       | <span data-ttu-id="6dcbd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dcbd-130">Type</span></span> | <span data-ttu-id="6dcbd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dcbd-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6dcbd-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dcbd-132">Authorization</span></span>  | <span data-ttu-id="6dcbd-133">string</span><span class="sxs-lookup"><span data-stu-id="6dcbd-133">string</span></span>  | <span data-ttu-id="6dcbd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6dcbd-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="6dcbd-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="6dcbd-137">string</span><span class="sxs-lookup"><span data-stu-id="6dcbd-137">string</span></span> | <span data-ttu-id="6dcbd-138">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="6dcbd-139">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="6dcbd-139">Values can be "text" or "html".</span></span> <span data-ttu-id="6dcbd-140">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="6dcbd-141">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="6dcbd-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dcbd-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-143">Request body</span></span>
<span data-ttu-id="6dcbd-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dcbd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dcbd-145">Response</span></span>

<span data-ttu-id="6dcbd-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="6dcbd-147">Especificar o parâmetro `$value` retorna o conteúdo da mensagem no formato MIME e não um recurso de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-147">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="6dcbd-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6dcbd-148">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="6dcbd-149">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="6dcbd-149">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="6dcbd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-150">Request</span></span>
<span data-ttu-id="6dcbd-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6dcbd-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dcbd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dcbd-153">C#</span><span class="sxs-lookup"><span data-stu-id="6dcbd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dcbd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dcbd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dcbd-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dcbd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dcbd-156">Java</span><span class="sxs-lookup"><span data-stu-id="6dcbd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6dcbd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dcbd-157">Response</span></span>
<span data-ttu-id="6dcbd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-2"></a><span data-ttu-id="6dcbd-161">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="6dcbd-161">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="6dcbd-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-162">Request</span></span>
<span data-ttu-id="6dcbd-163">O próximo exemplo usa um parâmetro de `$select` consulta para obter os cabeçalhos das mensagens de Internet de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-163">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="6dcbd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dcbd-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dcbd-165">C#</span><span class="sxs-lookup"><span data-stu-id="6dcbd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dcbd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dcbd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dcbd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dcbd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dcbd-168">Java</span><span class="sxs-lookup"><span data-stu-id="6dcbd-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6dcbd-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dcbd-169">Response</span></span>
<span data-ttu-id="6dcbd-170">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-170">Here is an example of the response.</span></span> <span data-ttu-id="6dcbd-171">Observação: O conjunto de cabeçalhos das mensagens no objeto de resposta é truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-171">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="6dcbd-172">Todas os cabeçalhos serão retornados de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-172">All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_headers",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```

### <a name="example-3"></a><span data-ttu-id="6dcbd-173">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="6dcbd-173">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="6dcbd-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-174">Request</span></span>

<span data-ttu-id="6dcbd-175">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter o **corpo** e o **uniqueBody** da mensagem especificada no formato do texto.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-175">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6dcbd-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dcbd-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dcbd-177">C#</span><span class="sxs-lookup"><span data-stu-id="6dcbd-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dcbd-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dcbd-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dcbd-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dcbd-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dcbd-180">Java</span><span class="sxs-lookup"><span data-stu-id="6dcbd-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6dcbd-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dcbd-181">Response</span></span>

<span data-ttu-id="6dcbd-182">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-182">Here is an example of the response.</span></span> <span data-ttu-id="6dcbd-183">Observação: a resposta inclui um `Preference-Applied: outlook.body-content-type` cabeçalho para reconhecer o `Prefer: outlook.body-content-type` cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-183">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
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
}
```

### <a name="example-4"></a><span data-ttu-id="6dcbd-184">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="6dcbd-184">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="6dcbd-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dcbd-185">Request</span></span>
<span data-ttu-id="6dcbd-186">O quarto exemplo obtém o conteúdo MIME de uma mensagem na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-186">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

#### <a name="response"></a><span data-ttu-id="6dcbd-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dcbd-187">Response</span></span>
<span data-ttu-id="6dcbd-188">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-188">The following is the response.</span></span> <span data-ttu-id="6dcbd-189">O conteúdo MIME começa com o `MIME-Version` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-189">The MIME content begins with the `MIME-Version` header.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_message_in_mime",
  "truncated": true,
  "@odata.type": "string"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 

MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```


## <a name="see-also"></a><span data-ttu-id="6dcbd-190">Confira também</span><span class="sxs-lookup"><span data-stu-id="6dcbd-190">See also</span></span>

- [<span data-ttu-id="6dcbd-191">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="6dcbd-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6dcbd-192">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="6dcbd-192">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
