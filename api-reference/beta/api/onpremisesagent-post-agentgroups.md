---
title: Atribuir onPremisesAgent a onPremisesAgentGroup
description: Atribua onPremisesAgent a onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 000385e1b2faad98bee217d2709f5516ea40b6b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342639"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="4d6af-103">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="4d6af-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d6af-104">Atribua um [onPremisesAgent](../resources/onpremisesagent.md) a um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6af-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d6af-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d6af-105">Permissions</span></span>

<span data-ttu-id="4d6af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d6af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d6af-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d6af-108">Permission type</span></span>                        | <span data-ttu-id="4d6af-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d6af-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d6af-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d6af-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d6af-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4d6af-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="4d6af-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d6af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d6af-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d6af-113">Not supported.</span></span> |
| <span data-ttu-id="4d6af-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d6af-114">Application</span></span>                            | <span data-ttu-id="4d6af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d6af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d6af-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d6af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4d6af-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6af-117">Request headers</span></span>

| <span data-ttu-id="4d6af-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4d6af-118">Name</span></span>          | <span data-ttu-id="4d6af-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d6af-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d6af-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d6af-120">Authorization</span></span> | <span data-ttu-id="4d6af-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4d6af-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d6af-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6af-122">Request body</span></span>

<span data-ttu-id="4d6af-123">No corpo da solicitação, forneça uma representação JSON de uma referência OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6af-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d6af-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d6af-124">Response</span></span>

<span data-ttu-id="4d6af-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d6af-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d6af-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d6af-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d6af-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6af-127">Request</span></span>

<span data-ttu-id="4d6af-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d6af-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d6af-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d6af-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d6af-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d6af-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d6af-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d6af-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="4d6af-132">No corpo da solicitação, forneça uma representação JSON de referência de OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6af-132">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="4d6af-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d6af-133">Response</span></span>

<span data-ttu-id="4d6af-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d6af-134">The following is an example of the response.</span></span>

> <span data-ttu-id="4d6af-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d6af-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
