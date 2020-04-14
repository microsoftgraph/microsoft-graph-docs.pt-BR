---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 30138336f98803f93dc6543d25dccf037783e29d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467087"
---
# <a name="create-message"></a><span data-ttu-id="97477-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="97477-103">Create Message</span></span>

<span data-ttu-id="97477-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97477-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97477-105">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="97477-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="97477-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97477-106">Permissions</span></span>
<span data-ttu-id="97477-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97477-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97477-109">Permission type</span></span>      | <span data-ttu-id="97477-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97477-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97477-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97477-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97477-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97477-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97477-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97477-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97477-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97477-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97477-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97477-115">Application</span></span> | <span data-ttu-id="97477-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97477-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97477-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97477-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="97477-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97477-118">Request headers</span></span>
| <span data-ttu-id="97477-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97477-119">Header</span></span>       | <span data-ttu-id="97477-120">Valor</span><span class="sxs-lookup"><span data-stu-id="97477-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97477-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="97477-121">Authorization</span></span>  | <span data-ttu-id="97477-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97477-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97477-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97477-124">Content-Type</span></span>  | <span data-ttu-id="97477-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97477-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97477-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97477-127">Request body</span></span>
<span data-ttu-id="97477-128">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="97477-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97477-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="97477-129">Response</span></span>

<span data-ttu-id="97477-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97477-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97477-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97477-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97477-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97477-132">Request</span></span>
<span data-ttu-id="97477-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97477-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97477-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="97477-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="97477-135">C#</span><span class="sxs-lookup"><span data-stu-id="97477-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97477-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97477-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="97477-137">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="97477-137">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="97477-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="97477-138">Response</span></span>
<span data-ttu-id="97477-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97477-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
