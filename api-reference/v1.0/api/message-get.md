---
title: Obter mensagem
description: Recupere as propriedades e os relacionamentos de um objeto message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ec663765c572230ad07e469b760c14b9dfd7c2e5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728689"
---
# <a name="get-message"></a><span data-ttu-id="5565c-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="5565c-103">Get message</span></span>

<span data-ttu-id="5565c-104">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="5565c-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="5565c-105">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5565c-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="5565c-106">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="5565c-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="5565c-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="5565c-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5565c-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5565c-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5565c-109">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="5565c-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="5565c-110">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="5565c-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="5565c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="5565c-111">Permissions</span></span>
<span data-ttu-id="5565c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5565c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5565c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5565c-114">Permission type</span></span>      | <span data-ttu-id="5565c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5565c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5565c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5565c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5565c-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5565c-117">Mail.Read</span></span>    |
|<span data-ttu-id="5565c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5565c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5565c-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5565c-119">Mail.Read</span></span>    |
|<span data-ttu-id="5565c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5565c-120">Application</span></span> | <span data-ttu-id="5565c-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5565c-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5565c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5565c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5565c-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5565c-123">Optional query parameters</span></span>
<span data-ttu-id="5565c-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5565c-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5565c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5565c-125">Request headers</span></span>
| <span data-ttu-id="5565c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="5565c-126">Name</span></span>       | <span data-ttu-id="5565c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5565c-127">Type</span></span> | <span data-ttu-id="5565c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5565c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5565c-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="5565c-129">Authorization</span></span>  | <span data-ttu-id="5565c-130">string</span><span class="sxs-lookup"><span data-stu-id="5565c-130">string</span></span>  | <span data-ttu-id="5565c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5565c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5565c-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5565c-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5565c-134">string</span><span class="sxs-lookup"><span data-stu-id="5565c-134">string</span></span> | <span data-ttu-id="5565c-135">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="5565c-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="5565c-136">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="5565c-136">Values can be "text" or "html".</span></span> <span data-ttu-id="5565c-137">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="5565c-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5565c-138">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5565c-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="5565c-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5565c-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5565c-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5565c-140">Request body</span></span>
<span data-ttu-id="5565c-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5565c-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5565c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5565c-142">Response</span></span>

<span data-ttu-id="5565c-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5565c-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5565c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5565c-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="5565c-145">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5565c-145">Request 1</span></span>
<span data-ttu-id="5565c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5565c-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5565c-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="5565c-147">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5565c-148">C#</span><span class="sxs-lookup"><span data-stu-id="5565c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5565c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5565c-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5565c-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5565c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5565c-151">Java</span><span class="sxs-lookup"><span data-stu-id="5565c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="5565c-152">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5565c-152">Response 1</span></span>
<span data-ttu-id="5565c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5565c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="5565c-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5565c-156">Request 2</span></span>
<span data-ttu-id="5565c-157">O próximo exemplo usa um parâmetro de `$select` consulta para obter os cabeçalhos das mensagens de Internet de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="5565c-157">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="5565c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="5565c-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5565c-159">C#</span><span class="sxs-lookup"><span data-stu-id="5565c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5565c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5565c-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5565c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5565c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5565c-162">Java</span><span class="sxs-lookup"><span data-stu-id="5565c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="5565c-163">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5565c-163">Response 2</span></span>
<span data-ttu-id="5565c-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5565c-164">Here is an example of the response.</span></span> <span data-ttu-id="5565c-165">Observação: O conjunto de cabeçalhos das mensagens no objeto de resposta é truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="5565c-165">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="5565c-166">Todas os cabeçalhos serão retornados de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5565c-166">All of the headers will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="5565c-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="5565c-167">See also</span></span>

- [<span data-ttu-id="5565c-168">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5565c-168">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5565c-169">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="5565c-169">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
