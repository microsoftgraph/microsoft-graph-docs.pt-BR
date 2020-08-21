---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fd866a3b57a159e53c6e288ba6f8a70a097877f6
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849391"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="d839a-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d839a-103">Delete outlookTaskGroup</span></span>

<span data-ttu-id="d839a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d839a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="d839a-105">Exclua o [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d839a-105">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d839a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d839a-106">Permissions</span></span>
<span data-ttu-id="d839a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d839a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d839a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d839a-109">Permission type</span></span>      | <span data-ttu-id="d839a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d839a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d839a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d839a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d839a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d839a-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d839a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d839a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d839a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d839a-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d839a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d839a-115">Application</span></span> | <span data-ttu-id="d839a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d839a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d839a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d839a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d839a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d839a-118">Request headers</span></span>
| <span data-ttu-id="d839a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d839a-119">Name</span></span>       | <span data-ttu-id="d839a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d839a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d839a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d839a-121">Authorization</span></span>  | <span data-ttu-id="d839a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d839a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d839a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d839a-124">Request body</span></span>
<span data-ttu-id="d839a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d839a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d839a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d839a-126">Response</span></span>

<span data-ttu-id="d839a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d839a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d839a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d839a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d839a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d839a-130">Request</span></span>
<span data-ttu-id="d839a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d839a-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d839a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d839a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="d839a-133">C#</span><span class="sxs-lookup"><span data-stu-id="d839a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d839a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d839a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d839a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d839a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d839a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d839a-136">Response</span></span>
<span data-ttu-id="d839a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d839a-137">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
