---
title: Excluir outlookTaskGroup
description: Exclua o outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 48854f8dab8c4b65ed983845c8e7cf6657f29890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988724"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="d6099-103">Excluir outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d6099-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6099-104">Exclua o [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d6099-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d6099-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6099-105">Permissions</span></span>
<span data-ttu-id="d6099-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6099-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6099-108">Permission type</span></span>      | <span data-ttu-id="d6099-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6099-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6099-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6099-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6099-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6099-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d6099-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6099-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6099-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6099-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d6099-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6099-114">Application</span></span> | <span data-ttu-id="d6099-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6099-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6099-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6099-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6099-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6099-117">Request headers</span></span>
| <span data-ttu-id="d6099-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d6099-118">Name</span></span>       | <span data-ttu-id="d6099-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6099-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6099-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6099-120">Authorization</span></span>  | <span data-ttu-id="d6099-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6099-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6099-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6099-123">Request body</span></span>
<span data-ttu-id="d6099-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6099-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6099-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6099-125">Response</span></span>

<span data-ttu-id="d6099-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6099-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6099-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6099-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6099-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6099-129">Request</span></span>
<span data-ttu-id="d6099-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6099-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6099-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6099-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6099-132">C#</span><span class="sxs-lookup"><span data-stu-id="d6099-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6099-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6099-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6099-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d6099-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6099-135">Java</span><span class="sxs-lookup"><span data-stu-id="d6099-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6099-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6099-136">Response</span></span>
<span data-ttu-id="d6099-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6099-137">Here is an example of the response.</span></span>
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
