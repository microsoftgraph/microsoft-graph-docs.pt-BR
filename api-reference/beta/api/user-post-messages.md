---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c15bfc0a29909b1e7a7ba27b5ac221c0d11f815
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509746"
---
# <a name="create-message"></a><span data-ttu-id="f7066-105">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="f7066-105">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7066-p102">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="f7066-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="f7066-109">Durante a criação de rascunho na mesma chamada **POST** , você pode:</span><span class="sxs-lookup"><span data-stu-id="f7066-109">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="f7066-110">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="f7066-110">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="f7066-111">Use um [mencionar](../resources/mention.md) chamar check-out de outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="f7066-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="f7066-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7066-112">Permissions</span></span>
<span data-ttu-id="f7066-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7066-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7066-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7066-115">Permission type</span></span>      | <span data-ttu-id="f7066-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7066-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7066-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7066-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f7066-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7066-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7066-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7066-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7066-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7066-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7066-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7066-121">Application</span></span> | <span data-ttu-id="f7066-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7066-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7066-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7066-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="f7066-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7066-124">Request headers</span></span>
| <span data-ttu-id="f7066-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7066-125">Header</span></span>       | <span data-ttu-id="f7066-126">Valor</span><span class="sxs-lookup"><span data-stu-id="f7066-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7066-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7066-127">Authorization</span></span>  | <span data-ttu-id="f7066-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7066-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7066-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7066-130">Content-Type</span></span>  | <span data-ttu-id="f7066-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f7066-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7066-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7066-132">Request body</span></span>
<span data-ttu-id="f7066-133">No corpo da solicitação, fornece uma representação JSON do objeto de [mensagem](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="f7066-133">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="f7066-134">Se você quiser usar **mencionar** chamar check-out de outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="f7066-134">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="f7066-135">Inclua a propriedade necessários **toRecipients** , a propriedade **menções** e propriedades de qualquer mensagem graváveis no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7066-135">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="f7066-136">Para cada mencionam na propriedade **menções** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="f7066-136">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="f7066-137">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="f7066-137">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="f7066-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7066-138">Response</span></span>

<span data-ttu-id="f7066-139">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto de [mensagem](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7066-139">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7066-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7066-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f7066-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="f7066-141">Request 1</span></span>
<span data-ttu-id="f7066-142">Aqui está um exemplo da solicitação para criar um rascunho de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="f7066-142">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="f7066-143">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="f7066-143">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="f7066-144">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="f7066-144">Response 1</span></span>
<span data-ttu-id="f7066-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7066-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="f7066-148">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="f7066-148">Request 2</span></span>
<span data-ttu-id="f7066-149">O exemplo a seguir mostra um email de rascunho por Randi Welch aos Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="f7066-149">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="f7066-150">A mensagem também inclui um mencionam de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="f7066-150">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="f7066-151">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="f7066-151">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="f7066-152">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="f7066-152">Response 2</span></span>
<span data-ttu-id="f7066-p107">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7066-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="f7066-156">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="f7066-156">Request 3</span></span>
<span data-ttu-id="f7066-157">O exemplo a seguir adiciona duas cabeçalhos de mensagem de Internet do cliente durante a criação de rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f7066-157">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="f7066-158">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="f7066-158">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="f7066-159">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="f7066-159">Response 3</span></span>
<span data-ttu-id="f7066-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7066-160">Here is an example of the response.</span></span> <span data-ttu-id="f7066-161">Observação: Os cabeçalhos de mensagens da Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="f7066-161">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="f7066-162">Também pode estar truncado no objeto response mostrado aqui para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="f7066-162">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="f7066-163">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7066-163">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f7066-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7066-164">See also</span></span>

- [<span data-ttu-id="f7066-165">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f7066-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f7066-166">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f7066-166">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f7066-167">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="f7066-167">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
