---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.
localization_priority: Priority
ms.openlocfilehash: 151c555e1195fcef243879c638fa36015395dc20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816230"
---
# <a name="create-message"></a><span data-ttu-id="0b5e1-105">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="0b5e1-105">Create Message</span></span>

<span data-ttu-id="0b5e1-p102">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="0b5e1-109">Ao criar o rascunho na mesma chamada de **POST**, você pode incluir um [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0b5e1-109">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b5e1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b5e1-110">Permissions</span></span>
<span data-ttu-id="0b5e1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b5e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b5e1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b5e1-113">Permission type</span></span>      | <span data-ttu-id="0b5e1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b5e1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b5e1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b5e1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0b5e1-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b5e1-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0b5e1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b5e1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b5e1-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b5e1-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0b5e1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b5e1-119">Application</span></span> | <span data-ttu-id="0b5e1-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b5e1-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b5e1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b5e1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="0b5e1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b5e1-122">Request headers</span></span>
| <span data-ttu-id="0b5e1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b5e1-123">Header</span></span>       | <span data-ttu-id="0b5e1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0b5e1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b5e1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b5e1-125">Authorization</span></span>  | <span data-ttu-id="0b5e1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0b5e1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b5e1-128">Content-Type</span></span>  | <span data-ttu-id="0b5e1-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0b5e1-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b5e1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b5e1-130">Request body</span></span>
<span data-ttu-id="0b5e1-131">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="0b5e1-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="0b5e1-132">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-132">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="0b5e1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b5e1-133">Response</span></span>

<span data-ttu-id="0b5e1-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-134">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b5e1-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b5e1-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="0b5e1-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="0b5e1-136">Request 1</span></span>
<span data-ttu-id="0b5e1-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-137">Here is an example of the request.</span></span>
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
<span data-ttu-id="0b5e1-138">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="0b5e1-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="0b5e1-139">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="0b5e1-139">Response 1</span></span>
<span data-ttu-id="0b5e1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="0b5e1-143">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="0b5e1-143">Request 2</span></span>
<span data-ttu-id="0b5e1-144">O exemplo a seguir adiciona duas cabeçalhos de mensagem de Internet do cliente durante a criação de rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-144">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="0b5e1-145">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="0b5e1-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="0b5e1-146">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="0b5e1-146">Response 2</span></span>
<span data-ttu-id="0b5e1-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-147">Here is an example of the response.</span></span> <span data-ttu-id="0b5e1-148">Observação: Os cabeçalhos de mensagens da Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-148">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="0b5e1-149">Também pode estar truncado no objeto response mostrado aqui para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-149">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="0b5e1-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b5e1-150">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0b5e1-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="0b5e1-151">See also</span></span>

- [<span data-ttu-id="0b5e1-152">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="0b5e1-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0b5e1-153">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="0b5e1-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": ""
}-->
