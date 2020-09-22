---
title: Excluir eventMessage
description: Exclua a eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 833c2af37ae92cccea5abf0c2eefc3efbaa75c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038736"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="fc731-103">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="fc731-103">Delete eventMessage</span></span>

<span data-ttu-id="fc731-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc731-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc731-105">Exclua a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="fc731-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc731-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc731-106">Permissions</span></span>
<span data-ttu-id="fc731-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc731-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc731-109">Permission type</span></span>      | <span data-ttu-id="fc731-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc731-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc731-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc731-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc731-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc731-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fc731-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc731-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc731-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc731-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fc731-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc731-115">Application</span></span> | <span data-ttu-id="fc731-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc731-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc731-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc731-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc731-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc731-118">Request headers</span></span>
| <span data-ttu-id="fc731-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc731-119">Name</span></span>       | <span data-ttu-id="fc731-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc731-120">Type</span></span> | <span data-ttu-id="fc731-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc731-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc731-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc731-122">Authorization</span></span>  | <span data-ttu-id="fc731-123">string</span><span class="sxs-lookup"><span data-stu-id="fc731-123">string</span></span>  | <span data-ttu-id="fc731-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc731-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc731-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc731-126">Request body</span></span>
<span data-ttu-id="fc731-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc731-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc731-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc731-128">Response</span></span>

<span data-ttu-id="fc731-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc731-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc731-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc731-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc731-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc731-132">Request</span></span>
<span data-ttu-id="fc731-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc731-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc731-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc731-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="fc731-135">C#</span><span class="sxs-lookup"><span data-stu-id="fc731-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc731-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc731-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc731-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc731-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc731-138">Java</span><span class="sxs-lookup"><span data-stu-id="fc731-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc731-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc731-139">Response</span></span>
<span data-ttu-id="fc731-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc731-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

