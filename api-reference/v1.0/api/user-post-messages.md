---
title: Criar mensagem
description: Criar um rascunho de uma nova mensagem no formato JSON ou MIME.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d10c07c433b3d8456c574519aa497fc163dde09
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645630"
---
# <a name="create-message"></a><span data-ttu-id="81782-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="81782-103">Create message</span></span>

<span data-ttu-id="81782-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81782-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81782-105">Criar um rascunho de uma nova [mensagem](../resources/message.md) no formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="81782-105">Create a draft of a new [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="81782-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="81782-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="81782-107">Incluir um [anexo](../resources/attachment.md) na **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="81782-107">Include an [attachment](../resources/attachment.md) to the **message**.</span></span>
- <span data-ttu-id="81782-108">[Atualizar](../api/message-update.md) o rascunho mais tarde para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem.</span><span class="sxs-lookup"><span data-stu-id="81782-108">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="81782-109">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="81782-109">When using MIME format:</span></span>
- <span data-ttu-id="81782-110">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81782-110">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="81782-111">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="81782-111">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="81782-112">Por padrão, esta operação salva o rascunho na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="81782-112">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="81782-113">[Enviar](/graph/api-reference/beta/api/message-send.md) o rascunho da mensagem em uma operação subsequente.</span><span class="sxs-lookup"><span data-stu-id="81782-113">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="81782-114">Como alternativa, [envie uma nova mensagem](../api/user-sendmail.md) em uma única operação ou crie um rascunho para [encaminhar](../api/message-createforward.md), [responder](../api/message-createreply.md) e [responder a todos](../api/message-createreplyall.md) a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="81782-114">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation, or create a draft to [forward](../api/message-createforward.md), [reply](../api/message-createreply.md) and [reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="81782-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="81782-115">Permissions</span></span>
<span data-ttu-id="81782-116">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="81782-116">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="81782-117">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81782-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81782-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81782-118">Permission type</span></span>      | <span data-ttu-id="81782-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81782-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81782-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81782-120">Delegated (work or school account)</span></span> | <span data-ttu-id="81782-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81782-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81782-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81782-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81782-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81782-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81782-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81782-124">Application</span></span> | <span data-ttu-id="81782-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81782-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81782-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81782-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="81782-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81782-127">Request headers</span></span>
| <span data-ttu-id="81782-128">Nome</span><span class="sxs-lookup"><span data-stu-id="81782-128">Name</span></span>       | <span data-ttu-id="81782-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="81782-129">Type</span></span> | <span data-ttu-id="81782-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="81782-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81782-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="81782-131">Authorization</span></span>  | <span data-ttu-id="81782-132">string</span><span class="sxs-lookup"><span data-stu-id="81782-132">string</span></span>  | <span data-ttu-id="81782-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81782-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81782-135">Content-Length</span><span class="sxs-lookup"><span data-stu-id="81782-135">Content-Length</span></span> | <span data-ttu-id="81782-136">number</span><span class="sxs-lookup"><span data-stu-id="81782-136">number</span></span> | <span data-ttu-id="81782-137">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81782-137">0. Required.</span></span> |
| <span data-ttu-id="81782-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81782-138">Content-Type</span></span> | <span data-ttu-id="81782-139">string</span><span class="sxs-lookup"><span data-stu-id="81782-139">string</span></span>  | <span data-ttu-id="81782-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81782-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="81782-142">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="81782-142">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81782-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81782-143">Request body</span></span>
<span data-ttu-id="81782-144">Ao usar o formato JSON, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="81782-144">When using JSON format, provide a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="81782-145">Ao especificar o corpo no formato MIME, forneça ao conteúdo MIME os cabeçalhos de mensagem da Internet aplicáveis ("Para", "CC", "CCO", "Assunto"), todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81782-145">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="81782-146">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="81782-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="81782-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="81782-147">Response</span></span>

<span data-ttu-id="81782-148">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81782-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="81782-149">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="81782-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="81782-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81782-150">Examples</span></span>
### <a name="example-1-create-a-new-message-draft-using-json-format"></a><span data-ttu-id="81782-151">Exemplo 1: Criar um novo rascunho de mensagem usando o formato JSON</span><span class="sxs-lookup"><span data-stu-id="81782-151">Example 1: Create a new message draft using JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="81782-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81782-152">Request</span></span> 
<span data-ttu-id="81782-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81782-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81782-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="81782-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="81782-155">C#</span><span class="sxs-lookup"><span data-stu-id="81782-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81782-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81782-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81782-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81782-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81782-158">Java</span><span class="sxs-lookup"><span data-stu-id="81782-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="81782-159">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="81782-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="81782-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="81782-160">Response</span></span> 
<span data-ttu-id="81782-p104">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="81782-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-message-draft-that-includes-custom-message-headers"></a><span data-ttu-id="81782-163">Exemplo 2: Criar rascunho de mensagem que inclui cabeçalhos de mensagem personalizados</span><span class="sxs-lookup"><span data-stu-id="81782-163">Example 2: Create message draft that includes custom message headers</span></span>
#### <a name="request"></a><span data-ttu-id="81782-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81782-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="81782-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="81782-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="81782-166">C#</span><span class="sxs-lookup"><span data-stu-id="81782-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81782-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81782-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81782-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81782-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81782-169">Java</span><span class="sxs-lookup"><span data-stu-id="81782-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="81782-170">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="81782-170">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="81782-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="81782-171">Response</span></span>
<span data-ttu-id="81782-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81782-172">Here is an example of the response.</span></span> <span data-ttu-id="81782-173">Observação: Os cabeçalhos das mensagens Internet não são retornados por padrão em uma resposta de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="81782-173">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="81782-174">O objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="81782-174">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="81782-175">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81782-175">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-create-a-new-message-draft-using-mime-format"></a><span data-ttu-id="81782-176">Exemplo 3: Criar um novo rascunho de mensagem usando o formato MIME</span><span class="sxs-lookup"><span data-stu-id="81782-176">Example 3: Create a new message draft using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="81782-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81782-177">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_create_draft_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```

#### <a name="response"></a><span data-ttu-id="81782-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="81782-178">Response</span></span>
<span data-ttu-id="81782-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81782-179">Here is an example of the response.</span></span>
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

<span data-ttu-id="81782-180">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="81782-180">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="81782-181">Confira também</span><span class="sxs-lookup"><span data-stu-id="81782-181">See also</span></span>

- [<span data-ttu-id="81782-182">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="81782-182">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="81782-183">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="81782-183">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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

