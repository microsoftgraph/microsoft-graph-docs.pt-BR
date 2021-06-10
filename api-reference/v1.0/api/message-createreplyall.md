---
title: 'message: createReplyAll'
description: Crie um rascunho para responder ao remetente e a todos os destinatários da mensagem especificada, no formato JSON ou MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2d1b3970995db5e3d678e0e1b6daeef6a72ee40b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870413"
---
# <a name="message-createreplyall"></a><span data-ttu-id="7f7ec-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="7f7ec-103">message: createReplyAll</span></span>

<span data-ttu-id="7f7ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f7ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f7ec-105">Crie um rascunho para responder ao remetente e [a](../resources/message.md) todos os destinatários de uma mensagem no formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-105">Create a draft to reply to the sender and all recipients of a [message](../resources/message.md) in either JSON or MIME format.</span></span> 

<span data-ttu-id="7f7ec-106">Ao usar o formato JSON:</span><span class="sxs-lookup"><span data-stu-id="7f7ec-106">When using JSON format:</span></span>
- <span data-ttu-id="7f7ec-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7f7ec-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7f7ec-109">Se a mensagem original especificar um destinatário na propriedade **replyTo,** por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deverá enviar a resposta aos destinatários nas propriedades **replyTo** e **toRecipients,** e não os destinatários nas propriedades **from** e **toRecipients.**</span><span class="sxs-lookup"><span data-stu-id="7f7ec-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the **replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 
- <span data-ttu-id="7f7ec-110">Você pode [atualizar o](../api/message-update.md) rascunho posteriormente para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-110">You can [update](../api/message-update.md) the draft later to add reply content to the **body** or change other message properties.</span></span>

<span data-ttu-id="7f7ec-111">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="7f7ec-111">When using MIME format:</span></span>
- <span data-ttu-id="7f7ec-112">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="7f7ec-113">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="7f7ec-114">[Enviar](../api/message-send.md) o rascunho da mensagem em uma operação subsequente.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-114">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="7f7ec-115">Como alternativa, [responda-tudo a uma mensagem](../api/message-replyall.md) em uma única ação.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-115">Alternatively, [reply-all to a message](../api/message-replyall.md) in a single action.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f7ec-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f7ec-116">Permissions</span></span>
<span data-ttu-id="7f7ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f7ec-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f7ec-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f7ec-119">Permission type</span></span>      | <span data-ttu-id="7f7ec-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f7ec-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f7ec-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f7ec-121">Delegated (work or school account)</span></span> | <span data-ttu-id="7f7ec-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f7ec-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f7ec-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f7ec-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f7ec-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f7ec-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f7ec-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f7ec-125">Application</span></span> | <span data-ttu-id="7f7ec-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f7ec-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f7ec-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7ec-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```

## <a name="request-headers"></a><span data-ttu-id="7f7ec-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7ec-128">Request headers</span></span>
| <span data-ttu-id="7f7ec-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7f7ec-129">Name</span></span>       | <span data-ttu-id="7f7ec-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f7ec-130">Type</span></span> | <span data-ttu-id="7f7ec-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f7ec-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="7f7ec-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f7ec-132">Authorization</span></span>  | <span data-ttu-id="7f7ec-133">string</span><span class="sxs-lookup"><span data-stu-id="7f7ec-133">string</span></span>  | <span data-ttu-id="7f7ec-134">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-134">Bearer {token}.</span></span> <span data-ttu-id="7f7ec-135">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7f7ec-135">Required</span></span> |
| <span data-ttu-id="7f7ec-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f7ec-136">Content-Type</span></span> | <span data-ttu-id="7f7ec-137">string</span><span class="sxs-lookup"><span data-stu-id="7f7ec-137">string</span></span>  | <span data-ttu-id="7f7ec-138">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-138">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="7f7ec-139">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f7ec-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7ec-140">Request body</span></span>
<span data-ttu-id="7f7ec-141">Esse método não exige um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-141">This method does not require a request body.</span></span> 

<span data-ttu-id="7f7ec-142">No entanto, para criar um rascunho replyAll usando o formato MIME, forneça o conteúdo MIME com os headers de mensagens da Internet aplicáveis, todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-142">However, for creating a replyAll draft using MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="7f7ec-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7ec-143">Response</span></span>

<span data-ttu-id="7f7ec-144">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-144">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="7f7ec-145">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="7f7ec-145">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="7f7ec-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f7ec-146">Examples</span></span>
### <a name="example-1-create-a-message-draft-in-json-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="7f7ec-147">Exemplo 1: Criar um rascunho de mensagem no formato JSON para responder tudo a uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="7f7ec-147">Example 1: Create a message draft in JSON format to reply-all to an existing message</span></span>
<span data-ttu-id="7f7ec-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7f7ec-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7ec-149">Request</span></span>
<span data-ttu-id="7f7ec-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f7ec-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7ec-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="c"></a>[<span data-ttu-id="7f7ec-152">C#</span><span class="sxs-lookup"><span data-stu-id="7f7ec-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f7ec-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f7ec-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f7ec-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f7ec-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f7ec-155">Java</span><span class="sxs-lookup"><span data-stu-id="7f7ec-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f7ec-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7ec-156">Response</span></span>
<span data-ttu-id="7f7ec-p104">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
### <a name="example-2-create-a-message-draft-in-mime-format-to-reply-all-to-an-existing-message"></a><span data-ttu-id="7f7ec-159">Exemplo 2: Criar um rascunho de mensagem no formato MIME para responder tudo a uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="7f7ec-159">Example 2: Create a message draft in MIME format to reply-all to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="7f7ec-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7ec-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_createreplyAll_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAH5JaLAAA=/createReplyAll
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```

##### <a name="response"></a><span data-ttu-id="7f7ec-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7ec-161">Response</span></span>
<span data-ttu-id="7f7ec-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-162">Here is an example of the response.</span></span>
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

<span data-ttu-id="7f7ec-163">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="7f7ec-163">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

