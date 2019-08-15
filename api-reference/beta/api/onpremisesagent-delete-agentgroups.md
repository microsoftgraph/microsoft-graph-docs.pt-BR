---
title: Remover o onpremisesAgent de um onPremisesAgentGroup
description: Remover um onpremisesAgent de um onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a7787ea75342fc45d37c925d2a2a0bde997268fb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414564"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="eb95a-103">Remover o onPremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="eb95a-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb95a-104">Remover um [onPremisesAgent](../resources/onpremisesagent.md) de um [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span><span class="sxs-lookup"><span data-stu-id="eb95a-104">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb95a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb95a-105">Permissions</span></span>

<span data-ttu-id="eb95a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb95a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb95a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb95a-108">Permission type</span></span>                        | <span data-ttu-id="eb95a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb95a-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb95a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb95a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb95a-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb95a-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="eb95a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb95a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb95a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb95a-113">Not supported.</span></span> |
| <span data-ttu-id="eb95a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb95a-114">Application</span></span>                            | <span data-ttu-id="eb95a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb95a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb95a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb95a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="eb95a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb95a-117">Request headers</span></span>

| <span data-ttu-id="eb95a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eb95a-118">Name</span></span>          | <span data-ttu-id="eb95a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb95a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eb95a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb95a-120">Authorization</span></span> | <span data-ttu-id="eb95a-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="eb95a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb95a-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb95a-122">Request body</span></span>

<span data-ttu-id="eb95a-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb95a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb95a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb95a-124">Response</span></span>

<span data-ttu-id="eb95a-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb95a-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb95a-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb95a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb95a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb95a-128">Request</span></span>

<span data-ttu-id="eb95a-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb95a-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eb95a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb95a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb95a-131">C#</span><span class="sxs-lookup"><span data-stu-id="eb95a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb95a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb95a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb95a-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eb95a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb95a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb95a-134">Response</span></span>

<span data-ttu-id="eb95a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb95a-135">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
