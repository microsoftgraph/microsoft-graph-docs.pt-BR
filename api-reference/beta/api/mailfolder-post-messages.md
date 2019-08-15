---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 23d90f21413ad7cb07b3911e49366f1bac9c3fe5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415222"
---
# <a name="create-message"></a><span data-ttu-id="30beb-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="30beb-103">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30beb-104">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="30beb-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="30beb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30beb-105">Permissions</span></span>
<span data-ttu-id="30beb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30beb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30beb-108">Permission type</span></span>      | <span data-ttu-id="30beb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30beb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30beb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30beb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30beb-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30beb-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="30beb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30beb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30beb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30beb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="30beb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30beb-114">Application</span></span> | <span data-ttu-id="30beb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30beb-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30beb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30beb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="30beb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-117">Request headers</span></span>
| <span data-ttu-id="30beb-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30beb-118">Header</span></span>       | <span data-ttu-id="30beb-119">Valor</span><span class="sxs-lookup"><span data-stu-id="30beb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30beb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="30beb-120">Authorization</span></span>  | <span data-ttu-id="30beb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30beb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="30beb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30beb-123">Content-Type</span></span>  | <span data-ttu-id="30beb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30beb-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30beb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-126">Request body</span></span>
<span data-ttu-id="30beb-127">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="30beb-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="30beb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="30beb-128">Response</span></span>

<span data-ttu-id="30beb-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30beb-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30beb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30beb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30beb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-131">Request</span></span>
<span data-ttu-id="30beb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30beb-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30beb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="30beb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30beb-134">C#</span><span class="sxs-lookup"><span data-stu-id="30beb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30beb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30beb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="30beb-136">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="30beb-136">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="30beb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="30beb-137">Response</span></span>
<span data-ttu-id="30beb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30beb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

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
