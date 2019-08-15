---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 79ffb11f70d30c34cba5e2219593cc4178d938ea
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414032"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="17fac-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="17fac-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17fac-104">Exclua o [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="17fac-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="17fac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17fac-105">Permissions</span></span>
<span data-ttu-id="17fac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17fac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17fac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17fac-108">Permission type</span></span>      | <span data-ttu-id="17fac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17fac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17fac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17fac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17fac-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17fac-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="17fac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17fac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17fac-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17fac-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="17fac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17fac-114">Application</span></span> | <span data-ttu-id="17fac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17fac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17fac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17fac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="17fac-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17fac-117">Request headers</span></span>
| <span data-ttu-id="17fac-118">Nome</span><span class="sxs-lookup"><span data-stu-id="17fac-118">Name</span></span>       | <span data-ttu-id="17fac-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="17fac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="17fac-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="17fac-120">Authorization</span></span>  | <span data-ttu-id="17fac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17fac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17fac-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17fac-123">Request body</span></span>
<span data-ttu-id="17fac-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17fac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17fac-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="17fac-125">Response</span></span>

<span data-ttu-id="17fac-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17fac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17fac-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17fac-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17fac-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17fac-129">Request</span></span>
<span data-ttu-id="17fac-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17fac-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17fac-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fac-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17fac-132">C#</span><span class="sxs-lookup"><span data-stu-id="17fac-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17fac-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fac-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17fac-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="17fac-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17fac-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17fac-135">Response</span></span>
<span data-ttu-id="17fac-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17fac-136">Here is an example of the response.</span></span>
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
