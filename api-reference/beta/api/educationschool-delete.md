---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fbb5742008b532c37bcd8c064d8b4097c4e12cf9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416223"
---
# <a name="delete-educationschool"></a><span data-ttu-id="180b2-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="180b2-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180b2-104">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="180b2-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="180b2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="180b2-105">Permissions</span></span>
<span data-ttu-id="180b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="180b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180b2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="180b2-108">Permission type</span></span>      | <span data-ttu-id="180b2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="180b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="180b2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="180b2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="180b2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="180b2-111">Not supported.</span></span>  |
|<span data-ttu-id="180b2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="180b2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="180b2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="180b2-113">Not supported.</span></span>  |
|<span data-ttu-id="180b2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="180b2-114">Application</span></span> | <span data-ttu-id="180b2-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180b2-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="180b2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="180b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="180b2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="180b2-117">Request headers</span></span>
| <span data-ttu-id="180b2-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="180b2-118">Header</span></span>       | <span data-ttu-id="180b2-119">Valor</span><span class="sxs-lookup"><span data-stu-id="180b2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="180b2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="180b2-120">Authorization</span></span>  | <span data-ttu-id="180b2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="180b2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="180b2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="180b2-123">Request body</span></span>
<span data-ttu-id="180b2-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="180b2-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="180b2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="180b2-125">Response</span></span>
<span data-ttu-id="180b2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="180b2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="180b2-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="180b2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="180b2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="180b2-129">Request</span></span>
<span data-ttu-id="180b2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="180b2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="180b2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="180b2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="180b2-132">C#</span><span class="sxs-lookup"><span data-stu-id="180b2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="180b2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="180b2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="180b2-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="180b2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="180b2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="180b2-135">Response</span></span>
<span data-ttu-id="180b2-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="180b2-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
