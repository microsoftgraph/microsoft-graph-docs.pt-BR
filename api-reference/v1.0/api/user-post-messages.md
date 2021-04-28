---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b2776e4708c6a5a72ee2f9c612f05f5f093b196f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054291"
---
# <a name="create-message"></a><span data-ttu-id="1d0e0-105">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="1d0e0-105">Create Message</span></span>

<span data-ttu-id="1d0e0-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d0e0-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d0e0-p102">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="1d0e0-110">Ao criar o rascunho na mesma chamada de **POST**, você pode incluir um [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1d0e0-110">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d0e0-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d0e0-111">Permissions</span></span>
<span data-ttu-id="1d0e0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d0e0-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d0e0-114">Permission type</span></span>      | <span data-ttu-id="1d0e0-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d0e0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d0e0-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d0e0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1d0e0-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d0e0-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d0e0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d0e0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d0e0-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d0e0-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d0e0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d0e0-120">Application</span></span> | <span data-ttu-id="1d0e0-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d0e0-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d0e0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0e0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="1d0e0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0e0-123">Request headers</span></span>
| <span data-ttu-id="1d0e0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d0e0-124">Header</span></span>       | <span data-ttu-id="1d0e0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1d0e0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d0e0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d0e0-126">Authorization</span></span>  | <span data-ttu-id="1d0e0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d0e0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d0e0-129">Content-Type</span></span>  | <span data-ttu-id="1d0e0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="1d0e0-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d0e0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0e0-131">Request body</span></span>
<span data-ttu-id="1d0e0-132">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1d0e0-132">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="1d0e0-133">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-133">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="1d0e0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0e0-134">Response</span></span>

<span data-ttu-id="1d0e0-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-135">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d0e0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d0e0-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1d0e0-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="1d0e0-137">Request 1</span></span>
<span data-ttu-id="1d0e0-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d0e0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0e0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="1d0e0-140">C#</span><span class="sxs-lookup"><span data-stu-id="1d0e0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d0e0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d0e0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d0e0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d0e0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d0e0-143">Java</span><span class="sxs-lookup"><span data-stu-id="1d0e0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1d0e0-144">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1d0e0-144">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="1d0e0-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="1d0e0-145">Response 1</span></span>
<span data-ttu-id="1d0e0-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-146">Here is an example of the response.</span></span> <span data-ttu-id="1d0e0-147">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="1d0e0-148">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="1d0e0-148">Request 2</span></span>
<span data-ttu-id="1d0e0-149">O próximo exemplo adiciona alguns cabeçalhos das mensagens de Internet de cliente ao criar um rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-149">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d0e0-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0e0-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
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
# <a name="c"></a>[<span data-ttu-id="1d0e0-151">C#</span><span class="sxs-lookup"><span data-stu-id="1d0e0-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d0e0-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d0e0-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d0e0-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d0e0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d0e0-154">Java</span><span class="sxs-lookup"><span data-stu-id="1d0e0-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1d0e0-155">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1d0e0-155">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="1d0e0-156">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="1d0e0-156">Response 2</span></span>
<span data-ttu-id="1d0e0-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-157">Here is an example of the response.</span></span> <span data-ttu-id="1d0e0-158">Observação: Os cabeçalhos das mensagens Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-158">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="1d0e0-159">O objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-159">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="1d0e0-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d0e0-160">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
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

## <a name="see-also"></a><span data-ttu-id="1d0e0-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="1d0e0-161">See also</span></span>

- [<span data-ttu-id="1d0e0-162">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1d0e0-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1d0e0-163">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1d0e0-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

