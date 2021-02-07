---
title: 'message: move'
description: Mover uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76880630d5faa0e09c4fa1efeb17dcf7c2c64615
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136077"
---
# <a name="message-move"></a><span data-ttu-id="308eb-104">message: move</span><span class="sxs-lookup"><span data-stu-id="308eb-104">message: move</span></span>

<span data-ttu-id="308eb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="308eb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="308eb-106">Mover uma mensagem para outra pasta na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="308eb-106">Move a message to another folder within the specified user's mailbox.</span></span> <span data-ttu-id="308eb-107">Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.</span><span class="sxs-lookup"><span data-stu-id="308eb-107">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="308eb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="308eb-108">Permissions</span></span>

<span data-ttu-id="308eb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="308eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="308eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="308eb-111">Permission type</span></span> | <span data-ttu-id="308eb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="308eb-112">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="308eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="308eb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="308eb-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308eb-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="308eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="308eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="308eb-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308eb-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="308eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="308eb-117">Application</span></span> | <span data-ttu-id="308eb-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308eb-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="308eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="308eb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="308eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="308eb-120">Request headers</span></span>

| <span data-ttu-id="308eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="308eb-121">Header</span></span> | <span data-ttu-id="308eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="308eb-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="308eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="308eb-123">Authorization</span></span> | <span data-ttu-id="308eb-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="308eb-124">`Bearer {token}`.</span></span> <span data-ttu-id="308eb-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="308eb-125">Required.</span></span> |
| <span data-ttu-id="308eb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="308eb-126">Content-Type</span></span> | <span data-ttu-id="308eb-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="308eb-127">`application/json`.</span></span> <span data-ttu-id="308eb-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="308eb-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="308eb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="308eb-129">Request body</span></span>

<span data-ttu-id="308eb-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="308eb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="308eb-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="308eb-131">Parameter</span></span>   | <span data-ttu-id="308eb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="308eb-132">Type</span></span> |<span data-ttu-id="308eb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="308eb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="308eb-134">destinationId</span><span class="sxs-lookup"><span data-stu-id="308eb-134">destinationId</span></span>|<span data-ttu-id="308eb-135">String</span><span class="sxs-lookup"><span data-stu-id="308eb-135">String</span></span>|<span data-ttu-id="308eb-136">A ID da pasta de destino ou um nome de pasta bem conhecido.</span><span class="sxs-lookup"><span data-stu-id="308eb-136">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="308eb-137">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="308eb-137">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="308eb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="308eb-138">Response</span></span>

<span data-ttu-id="308eb-139">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="308eb-139">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="308eb-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="308eb-140">Example</span></span>

<span data-ttu-id="308eb-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="308eb-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="308eb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="308eb-142">Request</span></span>

<span data-ttu-id="308eb-143">A solicitação a seguir move a mensagem especificada para a pasta Itens Excluídos, identificada por seu nome de pasta `deleteditems` conhecido.</span><span class="sxs-lookup"><span data-stu-id="308eb-143">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>

# <a name="http"></a>[<span data-ttu-id="308eb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="308eb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```
# <a name="c"></a>[<span data-ttu-id="308eb-145">C#</span><span class="sxs-lookup"><span data-stu-id="308eb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="308eb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="308eb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="308eb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="308eb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="308eb-148">Java</span><span class="sxs-lookup"><span data-stu-id="308eb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="308eb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="308eb-149">Response</span></span>

<span data-ttu-id="308eb-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="308eb-150">Here is an example of the response.</span></span>

> <span data-ttu-id="308eb-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="308eb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

