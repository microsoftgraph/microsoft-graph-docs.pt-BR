---
title: Obter mensagem
description: Recupere as propriedades e os relacionamentos de um objeto message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d15d1a148f56cb07b7526b6735385e4530abce41
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703809"
---
# <a name="get-message"></a><span data-ttu-id="8e8f5-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="8e8f5-103">Get message</span></span>

<span data-ttu-id="8e8f5-104">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="8e8f5-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="8e8f5-105">Você pode usar o `$value` parâmetro para [obter o conteúdo MIME de uma mensagem](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="8e8f5-105">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="8e8f5-106">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="8e8f5-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="8e8f5-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="8e8f5-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8e8f5-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8e8f5-109">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="8e8f5-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="8e8f5-110">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="8e8f5-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e8f5-111">Permissions</span></span>
<span data-ttu-id="8e8f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8f5-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e8f5-114">Permission type</span></span>      | <span data-ttu-id="8e8f5-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e8f5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e8f5-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e8f5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8e8f5-117">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8e8f5-117">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="8e8f5-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e8f5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e8f5-119">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8e8f5-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="8e8f5-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e8f5-120">Application</span></span> | <span data-ttu-id="8e8f5-121">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8e8f5-121">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e8f5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8f5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e8f5-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e8f5-123">Optional query parameters</span></span>
<span data-ttu-id="8e8f5-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e8f5-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f5-125">Request headers</span></span>
| <span data-ttu-id="8e8f5-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8e8f5-126">Name</span></span>       | <span data-ttu-id="8e8f5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e8f5-127">Type</span></span> | <span data-ttu-id="8e8f5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e8f5-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e8f5-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e8f5-129">Authorization</span></span>  | <span data-ttu-id="8e8f5-130">string</span><span class="sxs-lookup"><span data-stu-id="8e8f5-130">string</span></span>  | <span data-ttu-id="8e8f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e8f5-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8e8f5-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8e8f5-134">string</span><span class="sxs-lookup"><span data-stu-id="8e8f5-134">string</span></span> | <span data-ttu-id="8e8f5-135">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="8e8f5-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="8e8f5-136">Values can be "text" or "html".</span></span> <span data-ttu-id="8e8f5-137">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="8e8f5-138">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="8e8f5-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e8f5-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f5-140">Request body</span></span>
<span data-ttu-id="8e8f5-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e8f5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f5-142">Response</span></span>

<span data-ttu-id="8e8f5-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="8e8f5-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e8f5-144">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="8e8f5-145">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="8e8f5-145">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="8e8f5-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f5-146">Request</span></span>
<span data-ttu-id="8e8f5-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e8f5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8f5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e8f5-149">C#</span><span class="sxs-lookup"><span data-stu-id="8e8f5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e8f5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e8f5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e8f5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e8f5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e8f5-152">Java</span><span class="sxs-lookup"><span data-stu-id="8e8f5-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e8f5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f5-153">Response</span></span>
<span data-ttu-id="8e8f5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

### <a name="example-2"></a><span data-ttu-id="8e8f5-157">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="8e8f5-157">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="8e8f5-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f5-158">Request</span></span>
<span data-ttu-id="8e8f5-159">O próximo exemplo usa um parâmetro de `$select` consulta para obter os cabeçalhos das mensagens de Internet de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-159">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="8e8f5-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8f5-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e8f5-161">C#</span><span class="sxs-lookup"><span data-stu-id="8e8f5-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e8f5-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e8f5-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e8f5-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e8f5-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e8f5-164">Java</span><span class="sxs-lookup"><span data-stu-id="8e8f5-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e8f5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f5-165">Response</span></span>
<span data-ttu-id="8e8f5-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-166">Here is an example of the response.</span></span> <span data-ttu-id="8e8f5-167">Observação: O conjunto de cabeçalhos das mensagens no objeto de resposta é truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-167">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="8e8f5-168">Todas os cabeçalhos serão retornados de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-168">All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

### <a name="example-3"></a><span data-ttu-id="8e8f5-169">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="8e8f5-169">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="8e8f5-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8f5-170">Request</span></span>

<span data-ttu-id="8e8f5-171">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter o **corpo** e o **uniqueBody** da mensagem especificada no formato do texto.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-171">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e8f5-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8f5-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e8f5-173">C#</span><span class="sxs-lookup"><span data-stu-id="8e8f5-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e8f5-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e8f5-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e8f5-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e8f5-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e8f5-176">Java</span><span class="sxs-lookup"><span data-stu-id="8e8f5-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e8f5-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8f5-177">Response</span></span>

<span data-ttu-id="8e8f5-178">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-178">Here is an example of the response.</span></span> <span data-ttu-id="8e8f5-179">Observação: a resposta inclui um `Preference-Applied: outlook.body-content-type` cabeçalho para reconhecer o `Prefer: outlook.body-content-type` cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e8f5-179">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="8e8f5-180">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e8f5-180">See also</span></span>

- [<span data-ttu-id="8e8f5-181">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="8e8f5-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8e8f5-182">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="8e8f5-182">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
