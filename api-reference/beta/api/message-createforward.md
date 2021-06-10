---
title: 'message: createForward'
description: Crie um rascunho para encaminhar uma mensagem existente, no formato JSON ou MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 758ca460786eb7e59c41762f8dfa4209b20a62b9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870420"
---
# <a name="message-createforward"></a><span data-ttu-id="1fd36-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="1fd36-103">message: createForward</span></span>

<span data-ttu-id="1fd36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd36-105">Crie um rascunho para encaminhar uma mensagem [existente](../resources/message.md), no formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="1fd36-105">Create a draft to forward an existing [message](../resources/message.md), in either JSON or MIME format.</span></span>

<span data-ttu-id="1fd36-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="1fd36-106">When using JSON format, you can:</span></span> 
- <span data-ttu-id="1fd36-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1fd36-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="1fd36-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="1fd36-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="1fd36-109">Especifique `toRecipients` o parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1fd36-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="1fd36-110">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="1fd36-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="1fd36-111">[Atualizar](../api/message-update.md) o rascunho mais tarde para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1fd36-111">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="1fd36-112">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="1fd36-112">When using MIME format:</span></span>
- <span data-ttu-id="1fd36-113">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd36-113">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="1fd36-114">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="1fd36-114">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="1fd36-115">[Enviar](../api/message-send.md) o rascunho da mensagem em uma operação subsequente.</span><span class="sxs-lookup"><span data-stu-id="1fd36-115">[Send](../api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="1fd36-116">Como alternativa, [encaminhe uma mensagem](../api/message-forward.md) em uma única operação.</span><span class="sxs-lookup"><span data-stu-id="1fd36-116">Alternatively, [forward a message](../api/message-forward.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fd36-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fd36-117">Permissions</span></span>
<span data-ttu-id="1fd36-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd36-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd36-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fd36-120">Permission type</span></span>      | <span data-ttu-id="1fd36-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fd36-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fd36-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fd36-122">Delegated (work or school account)</span></span> | <span data-ttu-id="1fd36-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd36-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fd36-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fd36-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fd36-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd36-125">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fd36-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fd36-126">Application</span></span> | <span data-ttu-id="1fd36-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd36-127">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fd36-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd36-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="1fd36-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd36-129">Request headers</span></span>
| <span data-ttu-id="1fd36-130">Nome</span><span class="sxs-lookup"><span data-stu-id="1fd36-130">Name</span></span>       | <span data-ttu-id="1fd36-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd36-131">Type</span></span> | <span data-ttu-id="1fd36-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd36-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fd36-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fd36-133">Authorization</span></span>  | <span data-ttu-id="1fd36-134">string</span><span class="sxs-lookup"><span data-stu-id="1fd36-134">string</span></span>  | <span data-ttu-id="1fd36-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd36-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1fd36-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fd36-137">Content-Type</span></span> | <span data-ttu-id="1fd36-138">string</span><span class="sxs-lookup"><span data-stu-id="1fd36-138">string</span></span>  | <span data-ttu-id="1fd36-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd36-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="1fd36-141">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="1fd36-141">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd36-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd36-142">Request body</span></span>
<span data-ttu-id="1fd36-143">Para enviar um objeto JSON, forneça os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1fd36-143">To send a JSON object provide the following parameters.</span></span>

| <span data-ttu-id="1fd36-144">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1fd36-144">Parameter</span></span>    | <span data-ttu-id="1fd36-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd36-145">Type</span></span>   |<span data-ttu-id="1fd36-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd36-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd36-147">comment</span><span class="sxs-lookup"><span data-stu-id="1fd36-147">comment</span></span>|<span data-ttu-id="1fd36-148">String</span><span class="sxs-lookup"><span data-stu-id="1fd36-148">String</span></span>|<span data-ttu-id="1fd36-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="1fd36-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="1fd36-151">toRecipients</span><span class="sxs-lookup"><span data-stu-id="1fd36-151">toRecipients</span></span>|<span data-ttu-id="1fd36-152">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1fd36-152">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="1fd36-153">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="1fd36-153">The list of recipients.</span></span>|
|<span data-ttu-id="1fd36-154">mensagem</span><span class="sxs-lookup"><span data-stu-id="1fd36-154">message</span></span>|[<span data-ttu-id="1fd36-155">message</span><span class="sxs-lookup"><span data-stu-id="1fd36-155">message</span></span>](../resources/message.md)|<span data-ttu-id="1fd36-156">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd36-156">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="1fd36-157">Ao especificar o corpo no formato MIME, forneça ao conteúdo MIME os cabeçalhos de mensagem da Internet aplicáveis ("Para", "CC", "CCO", "Assunto"), todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd36-157">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="1fd36-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd36-158">Response</span></span>

<span data-ttu-id="1fd36-159">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd36-159">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="1fd36-160">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="1fd36-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="1fd36-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fd36-161">Examples</span></span>

### <a name="example-1-create-a-draft-message-in-json-format-to-forward-an-existing-message"></a><span data-ttu-id="1fd36-162">Exemplo 1: Criar uma mensagem de rascunho no formato JSON para encaminhar uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="1fd36-162">Example 1: Create a draft message in JSON format to forward an existing message</span></span>
<span data-ttu-id="1fd36-163">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1fd36-163">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1fd36-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd36-164">Request</span></span>
<span data-ttu-id="1fd36-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd36-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fd36-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd36-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```
# <a name="c"></a>[<span data-ttu-id="1fd36-167">C#</span><span class="sxs-lookup"><span data-stu-id="1fd36-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fd36-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fd36-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fd36-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fd36-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fd36-170">Java</span><span class="sxs-lookup"><span data-stu-id="1fd36-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1fd36-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd36-171">Response</span></span>
<span data-ttu-id="1fd36-p107">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="1fd36-p107">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```


### <a name="example-2-create-a-draft-message-in-mime-format-to-forward-an-existing-message"></a><span data-ttu-id="1fd36-174">Exemplo 2: Criar uma mensagem de rascunho no formato MIME para encaminhar uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="1fd36-174">Example 2: Create a draft message in MIME format to forward an existing message</span></span>

##### <a name="request"></a><span data-ttu-id="1fd36-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd36-175">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_createForward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1FeGNoYW5n
```

##### <a name="response"></a><span data-ttu-id="1fd36-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd36-176">Response</span></span>
<span data-ttu-id="1fd36-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd36-177">Here is an example of the response.</span></span>

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

<span data-ttu-id="1fd36-178">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="1fd36-178">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
