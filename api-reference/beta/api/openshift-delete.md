---
title: Excluir openShift
description: Excluir um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 871ab3e5b8beb01caf78bdc9aacadeef8dbc708c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010728"
---
# <a name="delete-openshift"></a><span data-ttu-id="93c94-103">Excluir openShift</span><span class="sxs-lookup"><span data-stu-id="93c94-103">Delete openShift</span></span>

<span data-ttu-id="93c94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93c94-105">Excluir um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="93c94-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93c94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93c94-106">Permissions</span></span>

<span data-ttu-id="93c94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93c94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93c94-109">Permission type</span></span>                        | <span data-ttu-id="93c94-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93c94-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93c94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93c94-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93c94-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c94-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="93c94-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93c94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93c94-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93c94-114">Not supported.</span></span> |
| <span data-ttu-id="93c94-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93c94-115">Application</span></span>                            | <span data-ttu-id="93c94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93c94-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93c94-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93c94-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="93c94-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93c94-118">Request headers</span></span>

| <span data-ttu-id="93c94-119">Nome</span><span class="sxs-lookup"><span data-stu-id="93c94-119">Name</span></span>          | <span data-ttu-id="93c94-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="93c94-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="93c94-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="93c94-121">Authorization</span></span> | <span data-ttu-id="93c94-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93c94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93c94-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93c94-124">Request body</span></span>

<span data-ttu-id="93c94-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93c94-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93c94-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c94-126">Response</span></span>

<span data-ttu-id="93c94-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93c94-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93c94-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93c94-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93c94-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93c94-130">Request</span></span>

<span data-ttu-id="93c94-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93c94-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93c94-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c94-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="93c94-133">C#</span><span class="sxs-lookup"><span data-stu-id="93c94-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c94-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c94-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c94-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c94-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93c94-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="93c94-136">Response</span></span>

<span data-ttu-id="93c94-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93c94-137">The following is an example of the response.</span></span>

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


