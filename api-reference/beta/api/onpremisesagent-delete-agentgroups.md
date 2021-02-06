---
title: Remover onpremisesAgent de um onPremisesAgentGroup
description: Remova um onpremisesAgent de um onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 41719b5431bf04759788b56973a2dc11c5113b71
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136483"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="753c0-103">Remover onPremisesAgent de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="753c0-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="753c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753c0-105">Remover um [onPremisesAgent](../resources/onpremisesagent.md) de [um onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span><span class="sxs-lookup"><span data-stu-id="753c0-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="753c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="753c0-106">Permissions</span></span>

<span data-ttu-id="753c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="753c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="753c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="753c0-109">Permission type</span></span>                        | <span data-ttu-id="753c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="753c0-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="753c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="753c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="753c0-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="753c0-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="753c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="753c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="753c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="753c0-114">Not supported.</span></span> |
| <span data-ttu-id="753c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="753c0-115">Application</span></span>                            | <span data-ttu-id="753c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="753c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="753c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="753c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="753c0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="753c0-118">Request headers</span></span>

| <span data-ttu-id="753c0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="753c0-119">Name</span></span>          | <span data-ttu-id="753c0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="753c0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="753c0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="753c0-121">Authorization</span></span> | <span data-ttu-id="753c0-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="753c0-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="753c0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="753c0-123">Request body</span></span>

<span data-ttu-id="753c0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="753c0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="753c0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="753c0-125">Response</span></span>

<span data-ttu-id="753c0-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="753c0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="753c0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="753c0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="753c0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="753c0-129">Request</span></span>

<span data-ttu-id="753c0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="753c0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="753c0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="753c0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="753c0-132">C#</span><span class="sxs-lookup"><span data-stu-id="753c0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="753c0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="753c0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="753c0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="753c0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="753c0-135">Java</span><span class="sxs-lookup"><span data-stu-id="753c0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/removeonpremisesagentfromanonpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="753c0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="753c0-136">Response</span></span>

<span data-ttu-id="753c0-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="753c0-137">The following is an example of the response.</span></span>

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



