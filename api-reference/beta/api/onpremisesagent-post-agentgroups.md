---
title: Atribuir onPremisesAgent ao onPremisesAgentGroup
description: Atribua onPremisesAgent ao onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3ab4e1ed97dec2968bfac63c38d6f2044d4dfc21
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038163"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="0846d-103">Atribuir onPremisesAgent ao onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="0846d-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="0846d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0846d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0846d-105">Atribua [um onPremisesAgent](../resources/onpremisesagent.md) a um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0846d-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0846d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0846d-106">Permissions</span></span>

<span data-ttu-id="0846d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0846d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0846d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0846d-109">Permission type</span></span>                        | <span data-ttu-id="0846d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0846d-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0846d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0846d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0846d-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0846d-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="0846d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0846d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0846d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0846d-114">Not supported.</span></span> |
| <span data-ttu-id="0846d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0846d-115">Application</span></span>                            | <span data-ttu-id="0846d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0846d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0846d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0846d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0846d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0846d-118">Request headers</span></span>

| <span data-ttu-id="0846d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0846d-119">Name</span></span>          | <span data-ttu-id="0846d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0846d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0846d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0846d-121">Authorization</span></span> | <span data-ttu-id="0846d-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0846d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0846d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0846d-123">Request body</span></span>

<span data-ttu-id="0846d-124">No corpo da solicitação, fornece uma representação JSON de uma referência OData a um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0846d-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0846d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0846d-125">Response</span></span>

<span data-ttu-id="0846d-126">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0846d-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0846d-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0846d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0846d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0846d-128">Request</span></span>

<span data-ttu-id="0846d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0846d-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0846d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0846d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="0846d-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0846d-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0846d-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0846d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0846d-133">No corpo da solicitação, fornece uma representação JSON da referência OData a um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0846d-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="0846d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0846d-134">Response</span></span>

<span data-ttu-id="0846d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0846d-135">The following is an example of the response.</span></span>

> <span data-ttu-id="0846d-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0846d-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



