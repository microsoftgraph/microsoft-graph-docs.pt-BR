---
title: Excluir eventMessage
description: Exclua a eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 04b85a8d34d242af712f55e4d255357ff93613ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422639"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="55852-103">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="55852-103">Delete eventMessage</span></span>

<span data-ttu-id="55852-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55852-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55852-105">Exclua a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="55852-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="55852-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55852-106">Permissions</span></span>
<span data-ttu-id="55852-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55852-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55852-109">Permission type</span></span>      | <span data-ttu-id="55852-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55852-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55852-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55852-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55852-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55852-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55852-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55852-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55852-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55852-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55852-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55852-115">Application</span></span> | <span data-ttu-id="55852-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55852-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55852-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55852-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="55852-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55852-118">Request headers</span></span>
| <span data-ttu-id="55852-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55852-119">Name</span></span>       | <span data-ttu-id="55852-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="55852-120">Type</span></span> | <span data-ttu-id="55852-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="55852-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55852-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="55852-122">Authorization</span></span>  | <span data-ttu-id="55852-123">string</span><span class="sxs-lookup"><span data-stu-id="55852-123">string</span></span>  | <span data-ttu-id="55852-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55852-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55852-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55852-126">Request body</span></span>
<span data-ttu-id="55852-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55852-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55852-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="55852-128">Response</span></span>

<span data-ttu-id="55852-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55852-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55852-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55852-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55852-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55852-132">Request</span></span>
<span data-ttu-id="55852-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55852-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55852-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="55852-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="55852-135">C#</span><span class="sxs-lookup"><span data-stu-id="55852-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55852-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55852-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55852-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55852-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55852-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="55852-138">Response</span></span>
<span data-ttu-id="55852-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55852-139">Here is an example of the response.</span></span> 
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
