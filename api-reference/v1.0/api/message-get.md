---
title: Obter mensagem
description: Recupere as propriedades e os relacionamentos de um objeto message.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13215ac951f9c23b80edf44fd5b57f33866ae386
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136154"
---
# <a name="get-message"></a><span data-ttu-id="cdd90-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="cdd90-103">Get message</span></span>

<span data-ttu-id="cdd90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdd90-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdd90-105">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="cdd90-105">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="cdd90-106">Você pode usar o `$value` parâmetro para [obter o conteúdo MIME de uma mensagem](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="cdd90-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="cdd90-107">Veja também um [exemplo](#example-4-get-mime-content) abaixo.</span><span class="sxs-lookup"><span data-stu-id="cdd90-107">See also an [example](#example-4-get-mime-content) below.</span></span>

<span data-ttu-id="cdd90-108">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="cdd90-108">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="cdd90-109">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="cdd90-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cdd90-110">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="cdd90-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cdd90-111">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="cdd90-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="cdd90-112">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="cdd90-112">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="cdd90-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdd90-113">Permissions</span></span>
<span data-ttu-id="cdd90-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd90-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd90-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdd90-116">Permission type</span></span>      | <span data-ttu-id="cdd90-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdd90-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd90-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdd90-118">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd90-119">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd90-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="cdd90-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdd90-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd90-121">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd90-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="cdd90-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdd90-122">Application</span></span> | <span data-ttu-id="cdd90-123">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd90-123">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd90-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd90-124">HTTP request</span></span>

<span data-ttu-id="cdd90-125">Para obter a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="cdd90-125">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="cdd90-126">Para obter o conteúdo MIME da mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="cdd90-126">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdd90-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cdd90-127">Optional query parameters</span></span>
<span data-ttu-id="cdd90-128">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd90-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="cdd90-129">Use o parâmetro `$value` para obter o conteúdo MIME de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="cdd90-129">Use the `$value` parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdd90-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-130">Request headers</span></span>
| <span data-ttu-id="cdd90-131">Nome</span><span class="sxs-lookup"><span data-stu-id="cdd90-131">Name</span></span>       | <span data-ttu-id="cdd90-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdd90-132">Type</span></span> | <span data-ttu-id="cdd90-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdd90-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cdd90-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdd90-134">Authorization</span></span>  | <span data-ttu-id="cdd90-135">string</span><span class="sxs-lookup"><span data-stu-id="cdd90-135">string</span></span>  | <span data-ttu-id="cdd90-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdd90-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdd90-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="cdd90-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="cdd90-139">string</span><span class="sxs-lookup"><span data-stu-id="cdd90-139">string</span></span> | <span data-ttu-id="cdd90-140">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="cdd90-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="cdd90-141">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="cdd90-141">Values can be "text" or "html".</span></span> <span data-ttu-id="cdd90-142">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="cdd90-142">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="cdd90-143">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="cdd90-143">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="cdd90-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cdd90-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd90-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-145">Request body</span></span>
<span data-ttu-id="cdd90-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdd90-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd90-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd90-147">Response</span></span>

<span data-ttu-id="cdd90-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd90-148">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="cdd90-149">Especificar o parâmetro `$value` retorna o conteúdo da mensagem no formato MIME e não um recurso de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="cdd90-149">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="cdd90-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cdd90-150">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="cdd90-151">Exemplo 1: Obter uma mensagem específica</span><span class="sxs-lookup"><span data-stu-id="cdd90-151">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="cdd90-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-152">Request</span></span>
<span data-ttu-id="cdd90-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdd90-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdd90-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd90-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="c"></a>[<span data-ttu-id="cdd90-155">C#</span><span class="sxs-lookup"><span data-stu-id="cdd90-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd90-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd90-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd90-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd90-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd90-158">Java</span><span class="sxs-lookup"><span data-stu-id="cdd90-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cdd90-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd90-159">Response</span></span>
<span data-ttu-id="cdd90-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdd90-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-internet-message-headers"></a><span data-ttu-id="cdd90-163">Exemplo 2: Obter cabeçalhos de mensagens da Internet</span><span class="sxs-lookup"><span data-stu-id="cdd90-163">Example 2: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="cdd90-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-164">Request</span></span>
<span data-ttu-id="cdd90-165">O próximo exemplo usa um parâmetro de `$select` consulta para obter os cabeçalhos das mensagens de Internet de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="cdd90-165">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="http"></a>[<span data-ttu-id="cdd90-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd90-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="cdd90-167">C#</span><span class="sxs-lookup"><span data-stu-id="cdd90-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd90-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd90-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd90-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd90-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd90-170">Java</span><span class="sxs-lookup"><span data-stu-id="cdd90-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cdd90-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd90-171">Response</span></span>
<span data-ttu-id="cdd90-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd90-172">Here is an example of the response.</span></span> <span data-ttu-id="cdd90-173">Observação: O conjunto de cabeçalhos das mensagens no objeto de resposta é truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="cdd90-173">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="cdd90-174">Todas os cabeçalhos serão retornados de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdd90-174">All of the headers will be returned from an actual call.</span></span>
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="cdd90-175">Exemplo 3: Obter o corpo da mensagem em formato de texto</span><span class="sxs-lookup"><span data-stu-id="cdd90-175">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="cdd90-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-176">Request</span></span>

<span data-ttu-id="cdd90-177">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter o **corpo** e o **uniqueBody** da mensagem especificada no formato do texto.</span><span class="sxs-lookup"><span data-stu-id="cdd90-177">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdd90-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd90-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="cdd90-179">C#</span><span class="sxs-lookup"><span data-stu-id="cdd90-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd90-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd90-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd90-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd90-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd90-182">Java</span><span class="sxs-lookup"><span data-stu-id="cdd90-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdd90-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd90-183">Response</span></span>

<span data-ttu-id="cdd90-184">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd90-184">Here is an example of the response.</span></span> <span data-ttu-id="cdd90-185">Observação: a resposta inclui um `Preference-Applied: outlook.body-content-type` cabeçalho para reconhecer o `Prefer: outlook.body-content-type` cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdd90-185">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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

### <a name="example-4-get-mime-content"></a><span data-ttu-id="cdd90-186">Exemplo 4: Obter conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="cdd90-186">Example 4: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="cdd90-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd90-187">Request</span></span>
<span data-ttu-id="cdd90-188">O quarto exemplo obtém o conteúdo MIME de uma mensagem na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="cdd90-188">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="cdd90-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd90-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="cdd90-190">C#</span><span class="sxs-lookup"><span data-stu-id="cdd90-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd90-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd90-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd90-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd90-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd90-193">Java</span><span class="sxs-lookup"><span data-stu-id="cdd90-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdd90-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd90-194">Response</span></span>
<span data-ttu-id="cdd90-195">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd90-195">The following is the response.</span></span> <span data-ttu-id="cdd90-196">O conteúdo MIME começa com o `MIME-Version` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="cdd90-196">The MIME content begins with the `MIME-Version` header.</span></span> 

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


## <a name="see-also"></a><span data-ttu-id="cdd90-197">Confira também</span><span class="sxs-lookup"><span data-stu-id="cdd90-197">See also</span></span>

- [<span data-ttu-id="cdd90-198">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="cdd90-198">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cdd90-199">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="cdd90-199">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
