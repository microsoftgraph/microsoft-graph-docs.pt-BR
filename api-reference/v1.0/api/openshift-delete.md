---
title: Excluir openShift
description: Excluir um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a3cebac6cf4e1ae3357e2ad7e0e3de3e11dc8f2d
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217217"
---
# <a name="delete-openshift"></a><span data-ttu-id="b1c02-103">Excluir openShift</span><span class="sxs-lookup"><span data-stu-id="b1c02-103">Delete openShift</span></span>

<span data-ttu-id="b1c02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1c02-105">Excluir um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c02-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c02-106">Permissions</span></span>

<span data-ttu-id="b1c02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1c02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1c02-109">Permission type</span></span>                        | <span data-ttu-id="b1c02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1c02-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b1c02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1c02-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1c02-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b1c02-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b1c02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1c02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c02-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c02-114">Not supported.</span></span> |
| <span data-ttu-id="b1c02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1c02-115">Application</span></span>                            | <span data-ttu-id="b1c02-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c02-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="b1c02-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b1c02-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b1c02-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="b1c02-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1c02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c02-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b1c02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c02-120">Request headers</span></span>

| <span data-ttu-id="b1c02-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b1c02-121">Name</span></span>          | <span data-ttu-id="b1c02-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c02-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b1c02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1c02-123">Authorization</span></span> | <span data-ttu-id="b1c02-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1c02-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1c02-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c02-126">Request body</span></span>

<span data-ttu-id="b1c02-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1c02-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1c02-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c02-128">Response</span></span>

<span data-ttu-id="b1c02-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c02-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1c02-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b1c02-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1c02-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c02-132">Request</span></span>

<span data-ttu-id="b1c02-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1c02-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1c02-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c02-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="b1c02-135">C#</span><span class="sxs-lookup"><span data-stu-id="b1c02-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1c02-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1c02-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1c02-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1c02-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1c02-138">Java</span><span class="sxs-lookup"><span data-stu-id="b1c02-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b1c02-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c02-139">Response</span></span>

<span data-ttu-id="b1c02-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c02-140">The following is an example of the response.</span></span>

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
