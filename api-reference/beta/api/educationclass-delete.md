---
title: Excluir educationClass
description: Exclua uma aula. Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 05b2a5c8e277ce506f6c46fe3821901d99ec523d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426952"
---
# <a name="delete-educationclass"></a><span data-ttu-id="fee6e-104">Excluir educationClass</span><span class="sxs-lookup"><span data-stu-id="fee6e-104">Delete educationClass</span></span>

<span data-ttu-id="fee6e-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fee6e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee6e-106">Exclua uma aula.</span><span class="sxs-lookup"><span data-stu-id="fee6e-106">Delete a class.</span></span> <span data-ttu-id="fee6e-107">Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.</span><span class="sxs-lookup"><span data-stu-id="fee6e-107">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fee6e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fee6e-108">Permissions</span></span>
<span data-ttu-id="fee6e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee6e-111">Permission type</span></span>      | <span data-ttu-id="fee6e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fee6e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fee6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee6e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fee6e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee6e-114">Not supported.</span></span>  |
|<span data-ttu-id="fee6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee6e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fee6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee6e-116">Not supported.</span></span>  |
|<span data-ttu-id="fee6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fee6e-117">Application</span></span> | <span data-ttu-id="fee6e-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fee6e-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fee6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee6e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fee6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee6e-120">Request headers</span></span>
| <span data-ttu-id="fee6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fee6e-121">Header</span></span>       | <span data-ttu-id="fee6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fee6e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fee6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee6e-123">Authorization</span></span>  | <span data-ttu-id="fee6e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee6e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fee6e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee6e-126">Request body</span></span>
<span data-ttu-id="fee6e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fee6e-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fee6e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee6e-128">Response</span></span>
<span data-ttu-id="fee6e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee6e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee6e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee6e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fee6e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee6e-132">Request</span></span>
<span data-ttu-id="fee6e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fee6e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fee6e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fee6e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="c"></a>[<span data-ttu-id="fee6e-135">C#</span><span class="sxs-lookup"><span data-stu-id="fee6e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fee6e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fee6e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fee6e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fee6e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fee6e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee6e-138">Response</span></span>
<span data-ttu-id="fee6e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fee6e-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
