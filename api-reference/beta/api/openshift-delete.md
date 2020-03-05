---
title: Excluir openShift
description: Excluir um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0489ff3ee4c79a385ee0c5e14f8e81698adbf7ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456422"
---
# <a name="delete-openshift"></a><span data-ttu-id="91a24-103">Excluir openShift</span><span class="sxs-lookup"><span data-stu-id="91a24-103">Delete openShift</span></span>

<span data-ttu-id="91a24-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91a24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91a24-105">Excluir um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="91a24-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91a24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="91a24-106">Permissions</span></span>

<span data-ttu-id="91a24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91a24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91a24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91a24-109">Permission type</span></span>                        | <span data-ttu-id="91a24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91a24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91a24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91a24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91a24-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a24-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="91a24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91a24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91a24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91a24-114">Not supported.</span></span> |
| <span data-ttu-id="91a24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91a24-115">Application</span></span>                            | <span data-ttu-id="91a24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91a24-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91a24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91a24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="91a24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91a24-118">Request headers</span></span>

| <span data-ttu-id="91a24-119">Nome</span><span class="sxs-lookup"><span data-stu-id="91a24-119">Name</span></span>          | <span data-ttu-id="91a24-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a24-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="91a24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91a24-121">Authorization</span></span> | <span data-ttu-id="91a24-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91a24-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91a24-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91a24-124">Request body</span></span>

<span data-ttu-id="91a24-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91a24-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91a24-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a24-126">Response</span></span>

<span data-ttu-id="91a24-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91a24-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91a24-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91a24-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91a24-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91a24-130">Request</span></span>

<span data-ttu-id="91a24-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a24-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91a24-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="91a24-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
```
# <a name="c"></a>[<span data-ttu-id="91a24-133">C#</span><span class="sxs-lookup"><span data-stu-id="91a24-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91a24-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91a24-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91a24-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91a24-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91a24-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a24-136">Response</span></span>

<span data-ttu-id="91a24-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91a24-137">The following is an example of the response.</span></span>

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
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
