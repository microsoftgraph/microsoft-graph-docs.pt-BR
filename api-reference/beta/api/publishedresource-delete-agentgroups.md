---
title: Remover o publishedResource de um onPremisesAgentGroup
description: Remover um objeto [publishedResource](../resources/publishedresource.md) de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d83be65fb44a68a2474ce7a6ed360960c6084a9c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412394"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="059a9-103">Remover o publishedResource de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="059a9-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="059a9-104">Remover um objeto [publishedResource](../resources/publishedresource.md) de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="059a9-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="059a9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="059a9-105">Permissions</span></span>

<span data-ttu-id="059a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="059a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="059a9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="059a9-108">Permission type</span></span>                        | <span data-ttu-id="059a9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="059a9-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="059a9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="059a9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="059a9-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="059a9-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="059a9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="059a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="059a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="059a9-113">Not supported.</span></span> |
| <span data-ttu-id="059a9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="059a9-114">Application</span></span>                            | <span data-ttu-id="059a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="059a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="059a9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="059a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="059a9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="059a9-117">Request headers</span></span>

| <span data-ttu-id="059a9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="059a9-118">Name</span></span>          | <span data-ttu-id="059a9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="059a9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="059a9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="059a9-120">Authorization</span></span> | <span data-ttu-id="059a9-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="059a9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="059a9-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="059a9-122">Request body</span></span>

<span data-ttu-id="059a9-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="059a9-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="059a9-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="059a9-124">Response</span></span>

<span data-ttu-id="059a9-125">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="059a9-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="059a9-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="059a9-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="059a9-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="059a9-127">Request</span></span>

<span data-ttu-id="059a9-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="059a9-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="059a9-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="059a9-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="059a9-130">C#</span><span class="sxs-lookup"><span data-stu-id="059a9-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="059a9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059a9-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="059a9-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="059a9-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="059a9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="059a9-133">Response</span></span>

<span data-ttu-id="059a9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="059a9-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
