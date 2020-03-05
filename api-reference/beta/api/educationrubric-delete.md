---
title: Excluir educationRubric
description: Excluir um objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7ce4f5f3f7de8f57499a13130a776302378500a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425846"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="48cb8-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="48cb8-103">Delete educationRubric</span></span>

<span data-ttu-id="48cb8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48cb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48cb8-105">Excluir um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="48cb8-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48cb8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="48cb8-106">Permissions</span></span>

<span data-ttu-id="48cb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48cb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48cb8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48cb8-109">Permission type</span></span>                        | <span data-ttu-id="48cb8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48cb8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48cb8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48cb8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48cb8-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48cb8-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="48cb8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48cb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48cb8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48cb8-114">Not supported.</span></span> |
| <span data-ttu-id="48cb8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48cb8-115">Application</span></span>                            | <span data-ttu-id="48cb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48cb8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48cb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48cb8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="48cb8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48cb8-118">Request headers</span></span>

| <span data-ttu-id="48cb8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="48cb8-119">Name</span></span>          | <span data-ttu-id="48cb8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="48cb8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48cb8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="48cb8-121">Authorization</span></span> | <span data-ttu-id="48cb8-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="48cb8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="48cb8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48cb8-123">Request body</span></span>

<span data-ttu-id="48cb8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48cb8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48cb8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="48cb8-125">Response</span></span>

<span data-ttu-id="48cb8-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48cb8-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48cb8-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48cb8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48cb8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48cb8-129">Request</span></span>

<span data-ttu-id="48cb8-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48cb8-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48cb8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="48cb8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="48cb8-132">C#</span><span class="sxs-lookup"><span data-stu-id="48cb8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48cb8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48cb8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48cb8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48cb8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48cb8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="48cb8-135">Response</span></span>

<span data-ttu-id="48cb8-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48cb8-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
