---
title: Remover o onpremisesAgent de um onPremisesAgentGroup
description: Remover um onpremisesAgent de um onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 28fd1d913332b4329c2b3184f76009ff8a7ccbc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036210"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="3703b-103">Remover o onPremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3703b-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="3703b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3703b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3703b-105">Remover um [onPremisesAgent](../resources/onpremisesagent.md) de um [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span><span class="sxs-lookup"><span data-stu-id="3703b-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3703b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3703b-106">Permissions</span></span>

<span data-ttu-id="3703b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3703b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3703b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3703b-109">Permission type</span></span>                        | <span data-ttu-id="3703b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3703b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3703b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3703b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3703b-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3703b-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="3703b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3703b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3703b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3703b-114">Not supported.</span></span> |
| <span data-ttu-id="3703b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3703b-115">Application</span></span>                            | <span data-ttu-id="3703b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3703b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3703b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3703b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3703b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3703b-118">Request headers</span></span>

| <span data-ttu-id="3703b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3703b-119">Name</span></span>          | <span data-ttu-id="3703b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3703b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3703b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3703b-121">Authorization</span></span> | <span data-ttu-id="3703b-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="3703b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3703b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3703b-123">Request body</span></span>

<span data-ttu-id="3703b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3703b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3703b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3703b-125">Response</span></span>

<span data-ttu-id="3703b-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3703b-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3703b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3703b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3703b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3703b-129">Request</span></span>

<span data-ttu-id="3703b-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3703b-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3703b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3703b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="3703b-132">C#</span><span class="sxs-lookup"><span data-stu-id="3703b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3703b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3703b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3703b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3703b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3703b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3703b-135">Response</span></span>

<span data-ttu-id="3703b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3703b-136">The following is an example of the response.</span></span>

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


