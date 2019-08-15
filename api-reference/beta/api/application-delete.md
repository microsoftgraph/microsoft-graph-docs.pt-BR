---
title: Excluir aplicativo
description: Exclui um aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 671f1c2774c1e9c75224bd7159d9b0685e44ab13
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408360"
---
# <a name="delete-application"></a><span data-ttu-id="fa470-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa470-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa470-104">Exclui um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fa470-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa470-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa470-105">Permissions</span></span>
<span data-ttu-id="fa470-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa470-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa470-108">Permission type</span></span>      | <span data-ttu-id="fa470-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa470-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa470-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa470-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa470-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa470-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa470-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa470-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa470-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa470-113">Not supported.</span></span>    |
|<span data-ttu-id="fa470-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa470-114">Application</span></span> | <span data-ttu-id="fa470-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa470-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa470-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa470-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa470-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa470-117">Request headers</span></span>
| <span data-ttu-id="fa470-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fa470-118">Name</span></span>       | <span data-ttu-id="fa470-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa470-119">Type</span></span> | <span data-ttu-id="fa470-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa470-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa470-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa470-121">Authorization</span></span>  | <span data-ttu-id="fa470-122">string</span><span class="sxs-lookup"><span data-stu-id="fa470-122">string</span></span>  | <span data-ttu-id="fa470-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa470-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa470-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa470-125">Request body</span></span>
<span data-ttu-id="fa470-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa470-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa470-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa470-127">Response</span></span>

<span data-ttu-id="fa470-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa470-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa470-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa470-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa470-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa470-131">Request</span></span>
<span data-ttu-id="fa470-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa470-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa470-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa470-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa470-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa470-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa470-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa470-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa470-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa470-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa470-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa470-137">Response</span></span>
<span data-ttu-id="fa470-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa470-138">Here is an example of the response.</span></span> 
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
