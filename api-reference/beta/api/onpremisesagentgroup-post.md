---
title: Criar onPremisesAgentGroup
description: Criar um novo objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dfce148cd74d01bd838b4d30c40cac8af145f35
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200275"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="4c3e5-103">Criar onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="4c3e5-103">Create onPremisesAgentGroup</span></span>

<span data-ttu-id="4c3e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c3e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c3e5-105">Criar um novo objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3e5-105">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c3e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c3e5-106">Permissions</span></span>

<span data-ttu-id="4c3e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c3e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c3e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c3e5-109">Permission type</span></span>                        | <span data-ttu-id="4c3e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c3e5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c3e5-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c3e5-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="4c3e5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c3e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c3e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-114">Not supported.</span></span> |
| <span data-ttu-id="4c3e5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c3e5-115">Application</span></span>                            | <span data-ttu-id="4c3e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c3e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c3e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="4c3e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c3e5-118">Request headers</span></span>

| <span data-ttu-id="4c3e5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4c3e5-119">Name</span></span>          | <span data-ttu-id="4c3e5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c3e5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4c3e5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c3e5-121">Authorization</span></span> | <span data-ttu-id="4c3e5-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4c3e5-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c3e5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c3e5-123">Request body</span></span>

<span data-ttu-id="4c3e5-124">No corpo da solicitação, forneça uma representação JSON de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3e5-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="4c3e5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c3e5-125">Response</span></span>

<span data-ttu-id="4c3e5-126">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-126">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c3e5-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c3e5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c3e5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c3e5-128">Request</span></span>

<span data-ttu-id="4c3e5-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c3e5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c3e5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascript"></a>[<span data-ttu-id="4c3e5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c3e5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c3e5-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c3e5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="4c3e5-133">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3e5-133">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="4c3e5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c3e5-134">Response</span></span>

<span data-ttu-id="4c3e5-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-135">The following is an example of the response.</span></span>

> <span data-ttu-id="4c3e5-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c3e5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
