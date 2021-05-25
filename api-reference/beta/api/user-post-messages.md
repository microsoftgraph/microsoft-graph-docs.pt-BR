---
title: Criar mensagem
description: Crie um rascunho de uma nova mensagem no formato JSON ou MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: acb10508eec31e39d5f631aee91dc3b85f964d3d
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645567"
---
# <a name="create-message"></a><span data-ttu-id="1cd83-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="1cd83-103">Create Message</span></span>

<span data-ttu-id="1cd83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cd83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cd83-105">Crie um rascunho de uma nova mensagem no formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="1cd83-105">Create a draft of a new message in either JSON or MIME format.</span></span>

<span data-ttu-id="1cd83-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="1cd83-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="1cd83-107">Inclua um [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1cd83-107">Include an [attachment](../resources/attachment.md).</span></span>
- <span data-ttu-id="1cd83-108">Use uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="1cd83-108">Use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>
- <span data-ttu-id="1cd83-109">[Atualize](../api/message-update.md) o rascunho posteriormente para adicionar conteúdo ao **corpo ou** alterar outras propriedades da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1cd83-109">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="1cd83-110">Ao usar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="1cd83-110">When using MIME format:</span></span>
- <span data-ttu-id="1cd83-111">Forneça os [headers](https://tools.ietf.org/html/rfc2076) de mensagens da Internet aplicáveis e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045), todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cd83-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="1cd83-112">Adicione quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="1cd83-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="1cd83-113">Por padrão, essa operação salva o rascunho na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="1cd83-113">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="1cd83-114">[Envie](/graph/api-reference/beta/api/message-send.md) a mensagem de rascunho em uma operação subsequente.</span><span class="sxs-lookup"><span data-stu-id="1cd83-114">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="1cd83-115">Como alternativa, [envie uma nova](../api/user-sendmail.md) mensagem em uma única ação ou [](../api/message-createreplyall.md) crie um [rascunho](../api/message-createforward.md)para encaminhar [,](../api/message-createreply.md) para responder ou para responder a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="1cd83-115">Alternatively, [send a new message](../api/user-sendmail.md) in a single action, or create a draft [to forward](../api/message-createforward.md), [to reply](../api/message-createreply.md) or [to reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cd83-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cd83-116">Permissions</span></span>
<span data-ttu-id="1cd83-117">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1cd83-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="1cd83-118">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cd83-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cd83-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cd83-119">Permission type</span></span>      | <span data-ttu-id="1cd83-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cd83-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cd83-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cd83-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1cd83-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cd83-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cd83-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cd83-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cd83-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cd83-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cd83-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cd83-125">Application</span></span> | <span data-ttu-id="1cd83-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cd83-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cd83-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cd83-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="1cd83-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-128">Request headers</span></span>
| <span data-ttu-id="1cd83-129">Nome</span><span class="sxs-lookup"><span data-stu-id="1cd83-129">Name</span></span>       | <span data-ttu-id="1cd83-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd83-130">Type</span></span> | <span data-ttu-id="1cd83-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd83-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cd83-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cd83-132">Authorization</span></span>  | <span data-ttu-id="1cd83-133">string</span><span class="sxs-lookup"><span data-stu-id="1cd83-133">string</span></span>  | <span data-ttu-id="1cd83-134">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="1cd83-134">Bearer {token}.</span></span>|
| <span data-ttu-id="1cd83-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1cd83-135">Content-Type</span></span> | <span data-ttu-id="1cd83-136">string</span><span class="sxs-lookup"><span data-stu-id="1cd83-136">string</span></span>  | <span data-ttu-id="1cd83-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cd83-p102">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="1cd83-139">Usar `application/json` para um objeto JSON e para conteúdo `text/plain` MIME</span><span class="sxs-lookup"><span data-stu-id="1cd83-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cd83-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-140">Request body</span></span>
<span data-ttu-id="1cd83-141">Ao usar o formato JSON, forneça uma representação JSON do [objeto message.](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="1cd83-141">When using JSON format, provide a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="1cd83-142">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis ("To", "CC", "BCC", "Subject"), todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cd83-142">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="1cd83-143">Para usar **a menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="1cd83-143">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="1cd83-144">Inclua a propriedade **required toRecipients,** a propriedade **mentions** e quaisquer propriedades de mensagem writable no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cd83-144">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="1cd83-145">Para cada menção na **propriedade mentions,** você deve especificar a **propriedade** mencionada.</span><span class="sxs-lookup"><span data-stu-id="1cd83-145">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="1cd83-146">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="1cd83-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>


## <a name="response"></a><span data-ttu-id="1cd83-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd83-147">Response</span></span>

<span data-ttu-id="1cd83-148">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cd83-148">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="1cd83-149">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará e a seguinte mensagem de erro: "Cadeia de caracteres `400 Bad request` base64 inválida para conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="1cd83-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="1cd83-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cd83-150">Examples</span></span>
### <a name="example-1-create-a-message-draft-in-json-format"></a><span data-ttu-id="1cd83-151">Exemplo 1: Criar um rascunho de mensagem no formato JSON</span><span class="sxs-lookup"><span data-stu-id="1cd83-151">Example 1: Create a message draft in JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="1cd83-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-152">Request</span></span>
<span data-ttu-id="1cd83-153">Aqui está um exemplo da solicitação para criar um rascunho de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="1cd83-153">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cd83-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cd83-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1cd83-155">C#</span><span class="sxs-lookup"><span data-stu-id="1cd83-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cd83-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cd83-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cd83-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cd83-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cd83-158">Java</span><span class="sxs-lookup"><span data-stu-id="1cd83-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1cd83-159">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1cd83-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="1cd83-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd83-160">Response</span></span>
<span data-ttu-id="1cd83-p103">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="1cd83-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-draft-message-that-includes-an--mention"></a><span data-ttu-id="1cd83-163">Exemplo 2: Criar uma mensagem de rascunho que inclui uma @-mention</span><span class="sxs-lookup"><span data-stu-id="1cd83-163">Example 2: Create a draft message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="1cd83-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-164">Request</span></span>
<span data-ttu-id="1cd83-165">O próximo exemplo mostra um rascunho de email de Randi Welch para Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="1cd83-165">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="1cd83-166">A mensagem também inclui uma menção de outra usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="1cd83-166">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="1cd83-167">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1cd83-167">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cd83-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cd83-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1cd83-169">C#</span><span class="sxs-lookup"><span data-stu-id="1cd83-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cd83-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cd83-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cd83-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cd83-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cd83-172">Java</span><span class="sxs-lookup"><span data-stu-id="1cd83-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-mentions-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="1cd83-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd83-173">Response</span></span>
<span data-ttu-id="1cd83-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cd83-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-create-a-draft-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="1cd83-177">Exemplo 3: Criar uma mensagem de rascunho que inclua os headers de mensagens da Internet personalizados</span><span class="sxs-lookup"><span data-stu-id="1cd83-177">Example 3: Create a draft message that includes custom Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="1cd83-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1cd83-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cd83-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1cd83-180">C#</span><span class="sxs-lookup"><span data-stu-id="1cd83-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cd83-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cd83-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cd83-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cd83-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cd83-183">Java</span><span class="sxs-lookup"><span data-stu-id="1cd83-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1cd83-184">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1cd83-184">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="1cd83-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd83-185">Response</span></span>
<span data-ttu-id="1cd83-186">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cd83-186">Here is an example of the response.</span></span> <span data-ttu-id="1cd83-187">Observação: Os cabeçalhos das mensagens Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="1cd83-187">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="1cd83-188">O objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1cd83-188">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="1cd83-189">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cd83-189">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-4-create-a-message-draft-in-mime-format"></a><span data-ttu-id="1cd83-190">Exemplo 4: Criar um rascunho de mensagem no formato MIME</span><span class="sxs-lookup"><span data-stu-id="1cd83-190">Example 4: Create a message draft in MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="1cd83-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd83-191">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_create_draft_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRv
```

#### <a name="response"></a><span data-ttu-id="1cd83-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd83-192">Response</span></span>
<span data-ttu-id="1cd83-193">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cd83-193">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

<span data-ttu-id="1cd83-194">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="1cd83-194">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

## <a name="see-also"></a><span data-ttu-id="1cd83-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="1cd83-195">See also</span></span>

- [<span data-ttu-id="1cd83-196">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1cd83-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1cd83-197">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1cd83-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1cd83-198">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="1cd83-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
