---
title: 'message: move'
description: Mova uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f6614d3769d2619854782776c061436622f1309
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961194"
---
# <a name="message-move"></a><span data-ttu-id="8ff6d-104">message: move</span><span class="sxs-lookup"><span data-stu-id="8ff6d-104">message: move</span></span>

> <span data-ttu-id="8ff6d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ff6d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ff6d-107">Mova uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-107">Move a message to a folder.</span></span> <span data-ttu-id="8ff6d-108">Isso cria uma nova cópia da mensagem na pasta de destino e remove a mensagem original.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-108">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff6d-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8ff6d-109">Permissions</span></span>

<span data-ttu-id="8ff6d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff6d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ff6d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff6d-112">Permission type</span></span> | <span data-ttu-id="8ff6d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff6d-113">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="8ff6d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff6d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff6d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff6d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ff6d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff6d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff6d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff6d-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ff6d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff6d-118">Application</span></span> | <span data-ttu-id="8ff6d-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff6d-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff6d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff6d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="8ff6d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff6d-121">Request headers</span></span>

| <span data-ttu-id="8ff6d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ff6d-122">Header</span></span> | <span data-ttu-id="8ff6d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8ff6d-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="8ff6d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff6d-124">Authorization</span></span> | <span data-ttu-id="8ff6d-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-125"></span></span> <span data-ttu-id="8ff6d-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-126">Required.</span></span> |
| <span data-ttu-id="8ff6d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ff6d-127">Content-Type</span></span> | <span data-ttu-id="8ff6d-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-128"></span></span> <span data-ttu-id="8ff6d-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff6d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff6d-130">Request body</span></span>

<span data-ttu-id="8ff6d-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ff6d-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8ff6d-132">Parameter</span></span>   | <span data-ttu-id="8ff6d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff6d-133">Type</span></span> |<span data-ttu-id="8ff6d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff6d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ff6d-135">DestinationId</span><span class="sxs-lookup"><span data-stu-id="8ff6d-135">DestinationId</span></span>|<span data-ttu-id="8ff6d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff6d-136">String</span></span>|<span data-ttu-id="8ff6d-137">O ID da pasta de destino, ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-137">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="8ff6d-138">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8ff6d-138">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8ff6d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff6d-139">Response</span></span>

<span data-ttu-id="8ff6d-140">Se tiver êxito, este método retornará `201 Created` código de resposta e um recurso de [mensagem](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-140">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff6d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff6d-141">Example</span></span>

<span data-ttu-id="8ff6d-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8ff6d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff6d-143">Request</span></span>

<span data-ttu-id="8ff6d-144">A solicitação a seguir move a mensagem especificada para a pasta Itens excluídos, identificada por seu nome de pasta conhecido `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-144">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="8ff6d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff6d-145">Response</span></span>

<span data-ttu-id="8ff6d-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-146">Here is an example of the response.</span></span>

> <span data-ttu-id="8ff6d-147">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8ff6d-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff6d-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#message",
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
  "tocPath": ""
}-->
