# <a name="get-message"></a><span data-ttu-id="5046e-101">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="5046e-101">Get message</span></span>

<span data-ttu-id="5046e-102">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="5046e-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="5046e-103">No momento, essa operação retorna o corpo da mensagem somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5046e-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="5046e-104">Há dois cenários em que um aplicativo pode obter mensagens da pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="5046e-104">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="5046e-105">Se o aplicativo tiver permissões de aplicativo ou,</span><span class="sxs-lookup"><span data-stu-id="5046e-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5046e-106">Se o aplicativo tiver as [permissões](#permissions) apropriadas delegadas de um usuário, e outro usuário tiver compartilhado uma pasta de email com o primeiro usuário ou, tiver dado acesso delegado a ele.</span><span class="sxs-lookup"><span data-stu-id="5046e-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5046e-107">Confira os [detalhes e um exemplo](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="5046e-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

<span data-ttu-id="5046e-108">Como o recurso **message** suporta [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="5046e-108">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="5046e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5046e-109">Permissions</span></span>
<span data-ttu-id="5046e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5046e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5046e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5046e-112">Permission type</span></span>      | <span data-ttu-id="5046e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5046e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5046e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5046e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5046e-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5046e-115">Mail.Read</span></span>    |
|<span data-ttu-id="5046e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5046e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5046e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5046e-117">Mail.Read</span></span>    |
|<span data-ttu-id="5046e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5046e-118">Application</span></span> | <span data-ttu-id="5046e-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5046e-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5046e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5046e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5046e-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5046e-121">Optional query parameters</span></span>
<span data-ttu-id="5046e-122">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5046e-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5046e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5046e-123">Request headers</span></span>
| <span data-ttu-id="5046e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5046e-124">Name</span></span>       | <span data-ttu-id="5046e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5046e-125">Type</span></span> | <span data-ttu-id="5046e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5046e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5046e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5046e-127">Authorization</span></span>  | <span data-ttu-id="5046e-128">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5046e-128">string</span></span>  | <span data-ttu-id="5046e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5046e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5046e-131">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5046e-131">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5046e-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="5046e-132">string</span></span> | <span data-ttu-id="5046e-133">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="5046e-133">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="5046e-134">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="5046e-134">Values can be "text" or "html".</span></span> <span data-ttu-id="5046e-135">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="5046e-135">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5046e-136">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5046e-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="5046e-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5046e-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5046e-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5046e-138">Request body</span></span>
<span data-ttu-id="5046e-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5046e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5046e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5046e-140">Response</span></span>

<span data-ttu-id="5046e-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5046e-141">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5046e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5046e-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="5046e-143">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5046e-143">Request 1</span></span>
<span data-ttu-id="5046e-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5046e-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="5046e-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5046e-145">Response 1</span></span>
<span data-ttu-id="5046e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5046e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="5046e-149">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5046e-149">Request 2</span></span>
<span data-ttu-id="5046e-150">O próximo exemplo usa um parâmetro de consulta `$select` para obter os cabeçalhos de mensagem de internet de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="5046e-150">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="5046e-151">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5046e-151">Response 2</span></span>
<span data-ttu-id="5046e-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5046e-152">Here is an example of the response.</span></span> <span data-ttu-id="5046e-153">Observação: O conjunto de cabeçalhos de mensagem no objeto response está truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="5046e-153">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="5046e-154">Todas os cabeçalhos serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5046e-154">All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="5046e-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="5046e-155">See also</span></span>

- [<span data-ttu-id="5046e-156">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5046e-156">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="5046e-157">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="5046e-157">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
