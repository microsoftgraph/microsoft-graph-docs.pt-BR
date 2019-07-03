---
title: 'message: move'
description: Mover uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: cbb2b24e7a5ad3ebfc0780bb18d394a0d0bda501
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455284"
---
# <a name="message-move"></a><span data-ttu-id="78629-104">message: move</span><span class="sxs-lookup"><span data-stu-id="78629-104">message: move</span></span>

<span data-ttu-id="78629-105">Mover uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="78629-105">Move a message to a folder.</span></span> <span data-ttu-id="78629-106">Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.</span><span class="sxs-lookup"><span data-stu-id="78629-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="78629-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78629-107">Permissions</span></span>

<span data-ttu-id="78629-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78629-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78629-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78629-110">Permission type</span></span> | <span data-ttu-id="78629-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78629-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="78629-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78629-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78629-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78629-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="78629-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78629-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78629-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78629-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="78629-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78629-116">Application</span></span> | <span data-ttu-id="78629-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78629-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78629-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78629-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="78629-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78629-119">Request headers</span></span>

| <span data-ttu-id="78629-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78629-120">Header</span></span> | <span data-ttu-id="78629-121">Valor</span><span class="sxs-lookup"><span data-stu-id="78629-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="78629-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78629-122">Authorization</span></span> | <span data-ttu-id="78629-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="78629-123">`Bearer {token}`.</span></span> <span data-ttu-id="78629-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78629-124">Required.</span></span> |
| <span data-ttu-id="78629-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78629-125">Content-Type</span></span> | <span data-ttu-id="78629-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="78629-126">`application/json`.</span></span> <span data-ttu-id="78629-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78629-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78629-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78629-128">Request body</span></span>

<span data-ttu-id="78629-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78629-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78629-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="78629-130">Parameter</span></span>   | <span data-ttu-id="78629-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78629-131">Type</span></span> |<span data-ttu-id="78629-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78629-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78629-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="78629-133">destinationId</span></span>|<span data-ttu-id="78629-134">String</span><span class="sxs-lookup"><span data-stu-id="78629-134">String</span></span>|<span data-ttu-id="78629-135">A ID da pasta de destino ou um nome de pasta bem conhecido.</span><span class="sxs-lookup"><span data-stu-id="78629-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="78629-136">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="78629-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="78629-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="78629-137">Response</span></span>

<span data-ttu-id="78629-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78629-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78629-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78629-139">Example</span></span>

<span data-ttu-id="78629-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="78629-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="78629-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78629-141">Request</span></span>

<span data-ttu-id="78629-142">A solicitação a seguir move a mensagem especificada para a pasta Itens Excluídos, identificada por seu nome de pasta `deleteditems` conhecido.</span><span class="sxs-lookup"><span data-stu-id="78629-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="78629-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="78629-143">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="78629-144">C#</span><span class="sxs-lookup"><span data-stu-id="78629-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78629-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="78629-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78629-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78629-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78629-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="78629-147">Response</span></span>

<span data-ttu-id="78629-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78629-148">Here is an example of the response.</span></span>

> <span data-ttu-id="78629-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78629-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="78629-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78629-150">All the properties will be returned from an actual call.</span></span>
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
