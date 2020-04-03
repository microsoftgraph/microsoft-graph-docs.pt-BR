---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6ad18eb72988318a8639c1d48120d2ba3320064f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123723"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="28543-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="28543-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="28543-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28543-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28543-105">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28543-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28543-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28543-106">Permissions</span></span>

<span data-ttu-id="28543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28543-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28543-109">Permission type</span></span>      | <span data-ttu-id="28543-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28543-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28543-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28543-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28543-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28543-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="28543-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28543-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28543-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="28543-114">Not supported</span></span> |
|<span data-ttu-id="28543-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28543-115">Application</span></span> | <span data-ttu-id="28543-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28543-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28543-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28543-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="28543-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28543-118">Request headers</span></span>

| <span data-ttu-id="28543-119">Nome</span><span class="sxs-lookup"><span data-stu-id="28543-119">Name</span></span> | <span data-ttu-id="28543-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="28543-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="28543-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="28543-121">Authorization</span></span> | <span data-ttu-id="28543-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28543-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28543-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28543-124">Content-Type</span></span>  | <span data-ttu-id="28543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28543-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="28543-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28543-126">Request body</span></span>
<span data-ttu-id="28543-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28543-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="28543-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="28543-128">Response</span></span>

<span data-ttu-id="28543-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28543-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28543-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28543-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28543-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28543-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="28543-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="28543-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="28543-134">C#</span><span class="sxs-lookup"><span data-stu-id="28543-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28543-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28543-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28543-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28543-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28543-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="28543-137">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
