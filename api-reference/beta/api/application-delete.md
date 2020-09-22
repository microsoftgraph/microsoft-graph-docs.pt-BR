---
title: Excluir aplicativo
description: Exclui um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 025d9d6b67c545ab49f3b76df6bdd6dd71bcb830
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192522"
---
# <a name="delete-application"></a><span data-ttu-id="e7d15-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d15-103">Delete application</span></span>

<span data-ttu-id="e7d15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d15-105">Exclui um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7d15-105">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d15-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d15-106">Permissions</span></span>
<span data-ttu-id="e7d15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d15-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d15-109">Permission type</span></span>      | <span data-ttu-id="e7d15-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7d15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7d15-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d15-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7d15-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e7d15-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d15-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d15-114">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7d15-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d15-115">Application</span></span> | <span data-ttu-id="e7d15-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d15-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7d15-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d15-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7d15-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d15-118">Request headers</span></span>
| <span data-ttu-id="e7d15-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7d15-119">Name</span></span>       | <span data-ttu-id="e7d15-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d15-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e7d15-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d15-121">Authorization</span></span> | <span data-ttu-id="e7d15-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d15-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7d15-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d15-124">Request body</span></span>
<span data-ttu-id="e7d15-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d15-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d15-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d15-126">Response</span></span>

<span data-ttu-id="e7d15-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d15-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7d15-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d15-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7d15-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d15-130">Request</span></span>
<span data-ttu-id="e7d15-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d15-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7d15-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d15-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="e7d15-133">C#</span><span class="sxs-lookup"><span data-stu-id="e7d15-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7d15-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7d15-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7d15-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7d15-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7d15-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d15-136">Response</span></span>
<span data-ttu-id="e7d15-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d15-137">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


