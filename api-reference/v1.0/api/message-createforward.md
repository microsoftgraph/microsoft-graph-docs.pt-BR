---
title: 'message: createForward'
description: Crie um rascunho para encaminhar uma mensagem existente, no formato JSON ou MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9892fb41a6115abfad0e7c19167911db533ad213
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645602"
---
# <a name="message-createforward"></a><span data-ttu-id="a2d3b-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="a2d3b-103">message: createForward</span></span>

<span data-ttu-id="a2d3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2d3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2d3b-105">Crie um rascunho para encaminhar uma mensagem [existente](../resources/message.md), no formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-105">Create a draft to forward an existing [message](../resources/message.md), in either JSON or MIME format.</span></span>

<span data-ttu-id="a2d3b-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="a2d3b-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="a2d3b-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="a2d3b-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a2d3b-109">Especifique `toRecipients` o parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="a2d3b-110">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a2d3b-111">[Atualize](../api/message-update.md) o rascunho posteriormente para adicionar conteúdo ao **corpo ou** alterar outras propriedades da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-111">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="a2d3b-112">Ao usar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="a2d3b-112">When using MIME format:</span></span>
- <span data-ttu-id="a2d3b-113">Forneça os [headers](https://tools.ietf.org/html/rfc2076) de mensagens da Internet aplicáveis e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045), todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-113">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="a2d3b-114">Adicione quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-114">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="a2d3b-115">[Envie](../api/message-send.md) a mensagem de rascunho em uma operação subsequente.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-115">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="a2d3b-116">Como alternativa, [encaminhe uma mensagem](../api/message-forward.md) em uma única operação.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-116">Alternatively, [forward a message](../api/message-forward.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2d3b-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2d3b-117">Permissions</span></span>
<span data-ttu-id="a2d3b-118">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-118">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="a2d3b-119">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2d3b-119">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2d3b-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2d3b-120">Permission type</span></span>      | <span data-ttu-id="a2d3b-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2d3b-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2d3b-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2d3b-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a2d3b-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2d3b-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2d3b-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2d3b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2d3b-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2d3b-125">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a2d3b-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2d3b-126">Application</span></span> | <span data-ttu-id="a2d3b-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2d3b-127">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2d3b-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2d3b-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="a2d3b-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2d3b-129">Request headers</span></span>

| <span data-ttu-id="a2d3b-130">Nome</span><span class="sxs-lookup"><span data-stu-id="a2d3b-130">Name</span></span>       | <span data-ttu-id="a2d3b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2d3b-131">Type</span></span> | <span data-ttu-id="a2d3b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2d3b-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2d3b-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2d3b-133">Authorization</span></span>  | <span data-ttu-id="a2d3b-134">string</span><span class="sxs-lookup"><span data-stu-id="a2d3b-134">string</span></span>  | <span data-ttu-id="a2d3b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2d3b-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2d3b-137">Content-Type</span></span> | <span data-ttu-id="a2d3b-138">string</span><span class="sxs-lookup"><span data-stu-id="a2d3b-138">string</span></span>  | <span data-ttu-id="a2d3b-139">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-139">Nature of the data in the body of an entity.</span></span> <br/> <span data-ttu-id="a2d3b-140">Use `application/json` para um objeto JSON e para conteúdo `text/plain` MIME.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2d3b-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2d3b-141">Request body</span></span>
<span data-ttu-id="a2d3b-142">Esse método não exige um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-142">This method does not require a request body.</span></span>

<span data-ttu-id="a2d3b-143">No entanto, para criar um rascunho de encaminhamento usando o formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis ("To", "CC", "BCC", "Subject"), todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-143">However, for creating a forward draft using MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span> 

## <a name="response"></a><span data-ttu-id="a2d3b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2d3b-144">Response</span></span>

<span data-ttu-id="a2d3b-145">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-145">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="a2d3b-146">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará e a seguinte mensagem de erro: "Cadeia de caracteres `400 Bad request` base64 inválida para conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="a2d3b-146">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="a2d3b-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2d3b-147">Examples</span></span>

### <a name="example-1-create-a-draft-message-in-json-format-to-forward-an-existing-message"></a><span data-ttu-id="a2d3b-148">Exemplo 1: Criar uma mensagem de rascunho no formato JSON para encaminhar uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="a2d3b-148">Example 1: Create a draft message in JSON format to forward an existing message</span></span>
<span data-ttu-id="a2d3b-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-149">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a2d3b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2d3b-150">Request</span></span>

<span data-ttu-id="a2d3b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2d3b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2d3b-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```
# <a name="c"></a>[<span data-ttu-id="a2d3b-153">C#</span><span class="sxs-lookup"><span data-stu-id="a2d3b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2d3b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2d3b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2d3b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2d3b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2d3b-156">Java</span><span class="sxs-lookup"><span data-stu-id="a2d3b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2d3b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2d3b-157">Response</span></span>

<span data-ttu-id="a2d3b-p105">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-a-draft-message-in-mime-format-to-forward-an-existing-message"></a><span data-ttu-id="a2d3b-160">Exemplo 2 Criar uma mensagem de rascunho no formato MIME para encaminhar uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="a2d3b-160">Example 2 Create a draft message in MIME format to forward an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="a2d3b-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2d3b-161">Request</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/createForward
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASF
```

##### <a name="response"></a><span data-ttu-id="a2d3b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2d3b-162">Response</span></span>
<span data-ttu-id="a2d3b-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-163">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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

<span data-ttu-id="a2d3b-164">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="a2d3b-164">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

