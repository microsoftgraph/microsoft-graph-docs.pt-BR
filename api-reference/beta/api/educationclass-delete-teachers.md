---
title: Remover professor
description: Remova um professor de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 471ef0bc3d545edfe47e2a0d8d526c11e9d05412
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427806"
---
# <a name="remove-teacher"></a><span data-ttu-id="651ba-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="651ba-103">Remove teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651ba-104">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="651ba-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="651ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="651ba-105">Permissions</span></span>

<span data-ttu-id="651ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="651ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="651ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="651ba-108">Permission type</span></span>                        | <span data-ttu-id="651ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="651ba-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="651ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="651ba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="651ba-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="651ba-111">Not supported.</span></span>                              |
| <span data-ttu-id="651ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="651ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="651ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="651ba-113">Not supported.</span></span>                              |
| <span data-ttu-id="651ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="651ba-114">Application</span></span>                            | <span data-ttu-id="651ba-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ba-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="651ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="651ba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="651ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="651ba-117">Request headers</span></span>

| <span data-ttu-id="651ba-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="651ba-118">Header</span></span>        | <span data-ttu-id="651ba-119">Valor</span><span class="sxs-lookup"><span data-stu-id="651ba-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="651ba-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="651ba-120">Authorization</span></span> | <span data-ttu-id="651ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="651ba-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="651ba-123">Request body</span></span>

<span data-ttu-id="651ba-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="651ba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="651ba-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="651ba-125">Response</span></span>

<span data-ttu-id="651ba-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="651ba-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="651ba-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="651ba-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="651ba-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="651ba-128">Request</span></span>

<span data-ttu-id="651ba-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="651ba-129">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="651ba-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="651ba-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="651ba-131">C#</span><span class="sxs-lookup"><span data-stu-id="651ba-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="651ba-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="651ba-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="651ba-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="651ba-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="651ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="651ba-134">Response</span></span>

<span data-ttu-id="651ba-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="651ba-135">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
