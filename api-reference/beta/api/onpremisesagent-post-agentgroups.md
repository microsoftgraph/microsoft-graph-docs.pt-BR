---
title: Atribuir onPremisesAgent a onPremisesAgentGroup
description: Atribua onPremisesAgent a onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 574de094395d44221ebc468e03cb7201d665594e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841168"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="0768e-103">Atribuir onPremisesAgent a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="0768e-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0768e-104">Atribua um [onPremisesAgent](../resources/onpremisesagent.md) a um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0768e-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0768e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0768e-105">Permissions</span></span>

<span data-ttu-id="0768e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0768e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0768e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0768e-108">Permission type</span></span>                        | <span data-ttu-id="0768e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0768e-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0768e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0768e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0768e-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0768e-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="0768e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0768e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0768e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0768e-113">Not supported.</span></span> |
| <span data-ttu-id="0768e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0768e-114">Application</span></span>                            | <span data-ttu-id="0768e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0768e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0768e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0768e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0768e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0768e-117">Request headers</span></span>

| <span data-ttu-id="0768e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0768e-118">Name</span></span>          | <span data-ttu-id="0768e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0768e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0768e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0768e-120">Authorization</span></span> | <span data-ttu-id="0768e-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0768e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0768e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0768e-122">Request body</span></span>

<span data-ttu-id="0768e-123">No corpo da solicitação, forneça uma representação JSON de uma referência OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0768e-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0768e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0768e-124">Response</span></span>

<span data-ttu-id="0768e-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0768e-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0768e-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0768e-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0768e-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0768e-127">Request</span></span>

<span data-ttu-id="0768e-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0768e-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```

<span data-ttu-id="0768e-129">No corpo da solicitação, forneça uma representação JSON de referência de OData para um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0768e-129">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="0768e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0768e-130">Response</span></span>

<span data-ttu-id="0768e-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0768e-131">The following is an example of the response.</span></span>

> <span data-ttu-id="0768e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0768e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
