---
title: Criar onPremisesAgentGroup
description: Criar um novo objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1771976abc56bb2b39850dcc925003df8965192e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878265"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="9d2dc-103">Criar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9d2dc-103">Create onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d2dc-104">Criar um novo objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="9d2dc-104">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d2dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d2dc-105">Permissions</span></span>

<span data-ttu-id="9d2dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d2dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d2dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d2dc-108">Permission type</span></span>                        | <span data-ttu-id="9d2dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d2dc-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d2dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d2dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d2dc-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9d2dc-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9d2dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d2dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d2dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-113">Not supported.</span></span> |
| <span data-ttu-id="9d2dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d2dc-114">Application</span></span>                            | <span data-ttu-id="9d2dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d2dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="9d2dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2dc-117">Request headers</span></span>

| <span data-ttu-id="9d2dc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9d2dc-118">Name</span></span>          | <span data-ttu-id="9d2dc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d2dc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9d2dc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d2dc-120">Authorization</span></span> | <span data-ttu-id="9d2dc-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9d2dc-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d2dc-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2dc-122">Request body</span></span>

<span data-ttu-id="9d2dc-123">No corpo da solicitação, forneça uma representação JSON de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="9d2dc-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="9d2dc-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d2dc-124">Response</span></span>

<span data-ttu-id="9d2dc-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-125">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d2dc-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d2dc-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d2dc-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2dc-127">Request</span></span>

<span data-ttu-id="9d2dc-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d2dc-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2dc-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d2dc-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d2dc-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d2dc-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9d2dc-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="9d2dc-132">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="9d2dc-132">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="9d2dc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d2dc-133">Response</span></span>

<span data-ttu-id="9d2dc-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9d2dc-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d2dc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "displayName": "New Group",
    "publishingType": "provisioning",
    "isDefault": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
