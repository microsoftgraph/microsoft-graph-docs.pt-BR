---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cc5534fbde3a3071f849c7f843e2ded7a3edc9db
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598350"
---
# <a name="create-message"></a><span data-ttu-id="9ccce-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="9ccce-103">Create Message</span></span>

<span data-ttu-id="9ccce-104">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="9ccce-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ccce-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ccce-105">Permissions</span></span>
<span data-ttu-id="9ccce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ccce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ccce-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ccce-108">Permission type</span></span>      | <span data-ttu-id="9ccce-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ccce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ccce-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ccce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ccce-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ccce-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ccce-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ccce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ccce-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ccce-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ccce-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ccce-114">Application</span></span> | <span data-ttu-id="9ccce-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ccce-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ccce-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ccce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="9ccce-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ccce-117">Request headers</span></span>
| <span data-ttu-id="9ccce-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ccce-118">Header</span></span>       | <span data-ttu-id="9ccce-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9ccce-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ccce-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ccce-120">Authorization</span></span>  | <span data-ttu-id="9ccce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ccce-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ccce-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ccce-123">Content-Type</span></span>  | <span data-ttu-id="9ccce-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ccce-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ccce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ccce-126">Request body</span></span>
<span data-ttu-id="9ccce-127">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="9ccce-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ccce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ccce-128">Response</span></span>

<span data-ttu-id="9ccce-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ccce-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ccce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ccce-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ccce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ccce-131">Request</span></span>
<span data-ttu-id="9ccce-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ccce-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
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
<span data-ttu-id="9ccce-133">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="9ccce-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9ccce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ccce-134">Response</span></span>
<span data-ttu-id="9ccce-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ccce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9ccce-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9ccce-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9ccce-139">Basic</span><span class="sxs-lookup"><span data-stu-id="9ccce-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ccce-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ccce-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_from_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
