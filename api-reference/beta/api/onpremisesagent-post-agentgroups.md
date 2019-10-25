---
title: Atribuir onPremisesAgent a onPremisesAgentGroup
description: Atribua onPremisesAgent a onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2f9aa40f974d2ddd1276dd9eb8c63727d9519ed
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726053"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="8e40f-103">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="8e40f-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e40f-104">Atribua um [onPremisesAgent](../resources/onpremisesagent.md) a um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8e40f-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e40f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e40f-105">Permissions</span></span>

<span data-ttu-id="8e40f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e40f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e40f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e40f-108">Permission type</span></span>                        | <span data-ttu-id="8e40f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e40f-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e40f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e40f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e40f-111">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e40f-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="8e40f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e40f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e40f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e40f-113">Not supported.</span></span> |
| <span data-ttu-id="8e40f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e40f-114">Application</span></span>                            | <span data-ttu-id="8e40f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e40f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e40f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e40f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8e40f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e40f-117">Request headers</span></span>

| <span data-ttu-id="8e40f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8e40f-118">Name</span></span>          | <span data-ttu-id="8e40f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e40f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e40f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e40f-120">Authorization</span></span> | <span data-ttu-id="8e40f-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8e40f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e40f-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e40f-122">Request body</span></span>

<span data-ttu-id="8e40f-123">No corpo da solicitação, forneça uma representação JSON de uma referência OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8e40f-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e40f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e40f-124">Response</span></span>

<span data-ttu-id="8e40f-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e40f-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e40f-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e40f-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e40f-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e40f-127">Request</span></span>

<span data-ttu-id="8e40f-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e40f-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e40f-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e40f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e40f-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e40f-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e40f-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e40f-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8e40f-132">No corpo da solicitação, forneça uma representação JSON de referência de OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8e40f-132">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="8e40f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e40f-133">Response</span></span>

<span data-ttu-id="8e40f-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e40f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="8e40f-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e40f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
