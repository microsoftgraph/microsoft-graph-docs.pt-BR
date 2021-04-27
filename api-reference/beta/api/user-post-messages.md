---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 60663e9ffa2c0b016d5667e7ce03f6eff151865e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049615"
---
# <a name="create-message"></a><span data-ttu-id="5085f-105">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="5085f-105">Create Message</span></span>

<span data-ttu-id="5085f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5085f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5085f-p102">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="5085f-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="5085f-110">Ao criar o rascunho na mesma **chamada POST,** você pode:</span><span class="sxs-lookup"><span data-stu-id="5085f-110">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="5085f-111">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="5085f-111">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="5085f-112">Usar uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="5085f-112">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="5085f-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="5085f-113">Permissions</span></span>
<span data-ttu-id="5085f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5085f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5085f-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5085f-116">Permission type</span></span>      | <span data-ttu-id="5085f-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5085f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5085f-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5085f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5085f-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085f-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5085f-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5085f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5085f-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085f-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5085f-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5085f-122">Application</span></span> | <span data-ttu-id="5085f-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085f-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5085f-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5085f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="5085f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5085f-125">Request headers</span></span>
| <span data-ttu-id="5085f-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5085f-126">Header</span></span>       | <span data-ttu-id="5085f-127">Valor</span><span class="sxs-lookup"><span data-stu-id="5085f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5085f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="5085f-128">Authorization</span></span>  | <span data-ttu-id="5085f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5085f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5085f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5085f-131">Content-Type</span></span>  | <span data-ttu-id="5085f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5085f-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5085f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5085f-133">Request body</span></span>
<span data-ttu-id="5085f-134">No corpo da solicitação, fornece uma representação JSON do [objeto message.](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="5085f-134">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="5085f-135">Se você quiser usar a **menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="5085f-135">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="5085f-136">Inclua a propriedade **required toRecipients,** a propriedade **mentions** e quaisquer propriedades de mensagem writable no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5085f-136">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="5085f-137">Para cada menção na **propriedade mentions,** você deve especificar a **propriedade** mencionada.</span><span class="sxs-lookup"><span data-stu-id="5085f-137">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="5085f-138">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="5085f-138">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="5085f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5085f-139">Response</span></span>

<span data-ttu-id="5085f-140">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5085f-140">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5085f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5085f-141">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="5085f-142">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5085f-142">Request 1</span></span>
<span data-ttu-id="5085f-143">Aqui está um exemplo da solicitação para criar um rascunho de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="5085f-143">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="5085f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5085f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
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
# <a name="c"></a>[<span data-ttu-id="5085f-145">C#</span><span class="sxs-lookup"><span data-stu-id="5085f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5085f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5085f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5085f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5085f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5085f-148">Java</span><span class="sxs-lookup"><span data-stu-id="5085f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5085f-149">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="5085f-149">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="5085f-150">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5085f-150">Response 1</span></span>
<span data-ttu-id="5085f-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5085f-151">Here is an example of the response.</span></span> <span data-ttu-id="5085f-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5085f-152">Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="5085f-153">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5085f-153">Request 2</span></span>
<span data-ttu-id="5085f-154">O próximo exemplo mostra um rascunho de email de Randi Welch para Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="5085f-154">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="5085f-155">A mensagem também inclui uma menção de outra usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="5085f-155">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="5085f-156">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="5085f-156">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="5085f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5085f-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="5085f-158">C#</span><span class="sxs-lookup"><span data-stu-id="5085f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5085f-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5085f-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5085f-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5085f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5085f-161">Java</span><span class="sxs-lookup"><span data-stu-id="5085f-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-mentions-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response-2"></a><span data-ttu-id="5085f-162">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5085f-162">Response 2</span></span>
<span data-ttu-id="5085f-p107">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5085f-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

##### <a name="request-3"></a><span data-ttu-id="5085f-166">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="5085f-166">Request 3</span></span>
<span data-ttu-id="5085f-167">O próximo exemplo adiciona alguns cabeçalhos das mensagens de Internet de cliente ao criar um rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="5085f-167">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>

# <a name="http"></a>[<span data-ttu-id="5085f-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="5085f-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
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
# <a name="c"></a>[<span data-ttu-id="5085f-169">C#</span><span class="sxs-lookup"><span data-stu-id="5085f-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5085f-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5085f-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5085f-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5085f-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5085f-172">Java</span><span class="sxs-lookup"><span data-stu-id="5085f-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5085f-173">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="5085f-173">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="5085f-174">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="5085f-174">Response 3</span></span>
<span data-ttu-id="5085f-175">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5085f-175">Here is an example of the response.</span></span> <span data-ttu-id="5085f-176">Observação: Os cabeçalhos das mensagens Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="5085f-176">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="5085f-177">O objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5085f-177">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="5085f-178">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5085f-178">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
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

## <a name="see-also"></a><span data-ttu-id="5085f-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="5085f-179">See also</span></span>

- [<span data-ttu-id="5085f-180">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5085f-180">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5085f-181">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="5085f-181">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5085f-182">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="5085f-182">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


