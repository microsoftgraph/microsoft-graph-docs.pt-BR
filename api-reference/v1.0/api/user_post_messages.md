# <a name="create-message"></a><span data-ttu-id="e47df-101">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="e47df-101">Create Message</span></span>

<span data-ttu-id="e47df-p101">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="e47df-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="e47df-105">Ao criar o rascunho na mesma chamada de **POST**, você pode incluir um [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e47df-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e47df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e47df-106">Permissions</span></span>
<span data-ttu-id="e47df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e47df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e47df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e47df-109">Permission type</span></span>      | <span data-ttu-id="e47df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e47df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e47df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e47df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e47df-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47df-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e47df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e47df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e47df-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47df-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e47df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e47df-115">Application</span></span> | <span data-ttu-id="e47df-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47df-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e47df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e47df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="e47df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e47df-118">Request headers</span></span>
| <span data-ttu-id="e47df-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e47df-119">Header</span></span>       | <span data-ttu-id="e47df-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e47df-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e47df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e47df-121">Authorization</span></span>  | <span data-ttu-id="e47df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e47df-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e47df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e47df-124">Content-Type</span></span>  | <span data-ttu-id="e47df-125">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="e47df-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e47df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e47df-126">Request body</span></span>
<span data-ttu-id="e47df-127">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="e47df-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="e47df-128">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="e47df-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e47df-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e47df-129">Response</span></span>

<span data-ttu-id="e47df-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e47df-130">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e47df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e47df-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e47df-132">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e47df-132">Request 1</span></span>
<span data-ttu-id="e47df-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e47df-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="e47df-134">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="e47df-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="e47df-135">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e47df-135">Response 1</span></span>
<span data-ttu-id="e47df-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e47df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="e47df-139">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e47df-139">Request 2</span></span>
<span data-ttu-id="e47df-140">O exemplo a seguir adiciona alguns cabeçalhos de mensagem de internet do cliente durante a criação do rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e47df-140">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="e47df-141">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="e47df-141">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="e47df-142">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e47df-142">Response 2</span></span>
<span data-ttu-id="e47df-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e47df-143">Here is an example of the response.</span></span> <span data-ttu-id="e47df-144">Observação: Cabeçalhos de mensagens da internet não são retornados por padrão em uma resposta do tipo POST.</span><span class="sxs-lookup"><span data-stu-id="e47df-144">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="e47df-145">O objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e47df-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e47df-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e47df-146">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e47df-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="e47df-147">See also</span></span>

- [<span data-ttu-id="e47df-148">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e47df-148">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e47df-149">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="e47df-149">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
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
