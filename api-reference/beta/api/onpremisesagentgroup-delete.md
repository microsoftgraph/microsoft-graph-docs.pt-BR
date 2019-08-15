---
title: Excluir onPremisesAgentGroup
description: Excluir um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e6a78a79c2eab50cdf035d2c17c4d11637e74b4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414530"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="74c99-103">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="74c99-103">Delete onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74c99-104">Excluir um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="74c99-104">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c99-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="74c99-105">Permissions</span></span>

<span data-ttu-id="74c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74c99-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74c99-108">Permission type</span></span>                        | <span data-ttu-id="74c99-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74c99-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74c99-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74c99-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74c99-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="74c99-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="74c99-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74c99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c99-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c99-113">Not supported.</span></span> |
| <span data-ttu-id="74c99-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c99-114">Application</span></span>                            | <span data-ttu-id="74c99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c99-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74c99-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74c99-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="74c99-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74c99-117">Request headers</span></span>

| <span data-ttu-id="74c99-118">Nome</span><span class="sxs-lookup"><span data-stu-id="74c99-118">Name</span></span>          | <span data-ttu-id="74c99-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c99-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="74c99-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="74c99-120">Authorization</span></span> | <span data-ttu-id="74c99-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="74c99-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="74c99-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74c99-122">Request body</span></span>

<span data-ttu-id="74c99-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74c99-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c99-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c99-124">Response</span></span>

<span data-ttu-id="74c99-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74c99-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74c99-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="74c99-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74c99-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74c99-128">Request</span></span>

<span data-ttu-id="74c99-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74c99-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74c99-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c99-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74c99-131">C#</span><span class="sxs-lookup"><span data-stu-id="74c99-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74c99-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c99-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74c99-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="74c99-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74c99-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c99-134">Response</span></span>

<span data-ttu-id="74c99-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74c99-135">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
