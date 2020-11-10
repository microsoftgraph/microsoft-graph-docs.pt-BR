---
title: Excluir eventMessage
description: Exclua a eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ef524c051e0d2052c8afe50c36a9d366e8ac8303
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954688"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="1853c-103">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="1853c-103">Delete eventMessage</span></span>

<span data-ttu-id="1853c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1853c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1853c-105">Exclua a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="1853c-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="1853c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1853c-106">Permissions</span></span>
<span data-ttu-id="1853c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1853c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1853c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1853c-109">Permission type</span></span>      | <span data-ttu-id="1853c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1853c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1853c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1853c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1853c-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1853c-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1853c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1853c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1853c-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1853c-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1853c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1853c-115">Application</span></span> | <span data-ttu-id="1853c-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1853c-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1853c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1853c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1853c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1853c-118">Request headers</span></span>
| <span data-ttu-id="1853c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1853c-119">Name</span></span>       | <span data-ttu-id="1853c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1853c-120">Type</span></span> | <span data-ttu-id="1853c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1853c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1853c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1853c-122">Authorization</span></span>  | <span data-ttu-id="1853c-123">string</span><span class="sxs-lookup"><span data-stu-id="1853c-123">string</span></span>  | <span data-ttu-id="1853c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1853c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1853c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1853c-126">Request body</span></span>
<span data-ttu-id="1853c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1853c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1853c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1853c-128">Response</span></span>

<span data-ttu-id="1853c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1853c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1853c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1853c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1853c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1853c-132">Request</span></span>
<span data-ttu-id="1853c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1853c-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1853c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1853c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="1853c-135">C#</span><span class="sxs-lookup"><span data-stu-id="1853c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1853c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1853c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1853c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1853c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1853c-138">Java</span><span class="sxs-lookup"><span data-stu-id="1853c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1853c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1853c-139">Response</span></span>
<span data-ttu-id="1853c-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1853c-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


