---
title: Excluir openShift
description: Excluir um objeto openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70fd651899010c827a2fbfed70776c5a1fe07a6b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962819"
---
# <a name="delete-openshift"></a><span data-ttu-id="41aaf-103">Excluir openShift</span><span class="sxs-lookup"><span data-stu-id="41aaf-103">Delete openShift</span></span>

<span data-ttu-id="41aaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41aaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41aaf-105">Excluir um objeto [openShift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="41aaf-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41aaf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41aaf-106">Permissions</span></span>

<span data-ttu-id="41aaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41aaf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41aaf-109">Permission type</span></span>                        | <span data-ttu-id="41aaf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41aaf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41aaf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41aaf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41aaf-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41aaf-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="41aaf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41aaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41aaf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41aaf-114">Not supported.</span></span> |
| <span data-ttu-id="41aaf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41aaf-115">Application</span></span>                            | <span data-ttu-id="41aaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41aaf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41aaf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41aaf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="41aaf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41aaf-118">Request headers</span></span>

| <span data-ttu-id="41aaf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="41aaf-119">Name</span></span>          | <span data-ttu-id="41aaf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="41aaf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="41aaf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41aaf-121">Authorization</span></span> | <span data-ttu-id="41aaf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41aaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41aaf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41aaf-124">Request body</span></span>

<span data-ttu-id="41aaf-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41aaf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41aaf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="41aaf-126">Response</span></span>

<span data-ttu-id="41aaf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41aaf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41aaf-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41aaf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41aaf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41aaf-130">Request</span></span>

<span data-ttu-id="41aaf-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41aaf-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41aaf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="41aaf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="41aaf-133">C#</span><span class="sxs-lookup"><span data-stu-id="41aaf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41aaf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41aaf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41aaf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41aaf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41aaf-136">Java</span><span class="sxs-lookup"><span data-stu-id="41aaf-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41aaf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="41aaf-137">Response</span></span>

<span data-ttu-id="41aaf-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41aaf-138">The following is an example of the response.</span></span>

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


