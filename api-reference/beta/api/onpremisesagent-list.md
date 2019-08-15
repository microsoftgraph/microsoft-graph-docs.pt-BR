---
title: Listar onPremisesAgents
description: Recupere uma lista de onPremisesAgents.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a3c66df35c9948fe700799a47b529101f7aec4ad
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414522"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="725b5-103">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="725b5-103">List onPremisesAgents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="725b5-104">Recupere uma lista de objetos [onPremisesAgent](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="725b5-104">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="725b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="725b5-105">Permissions</span></span>

<span data-ttu-id="725b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="725b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="725b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="725b5-108">Permission type</span></span>                        | <span data-ttu-id="725b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="725b5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="725b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="725b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="725b5-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="725b5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="725b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="725b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="725b5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="725b5-113">Not supported.</span></span> |
| <span data-ttu-id="725b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="725b5-114">Application</span></span>                            | <span data-ttu-id="725b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="725b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="725b5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="725b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="725b5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="725b5-117">Optional query parameters</span></span>

<span data-ttu-id="725b5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="725b5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="725b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="725b5-119">Request headers</span></span>

| <span data-ttu-id="725b5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="725b5-120">Name</span></span>      |<span data-ttu-id="725b5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="725b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="725b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="725b5-122">Authorization</span></span> | <span data-ttu-id="725b5-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="725b5-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="725b5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="725b5-124">Request body</span></span>

<span data-ttu-id="725b5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="725b5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="725b5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="725b5-126">Response</span></span>

<span data-ttu-id="725b5-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="725b5-127">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="725b5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="725b5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="725b5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="725b5-129">Request</span></span>

<span data-ttu-id="725b5-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="725b5-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="725b5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="725b5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="725b5-132">C#</span><span class="sxs-lookup"><span data-stu-id="725b5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="725b5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="725b5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="725b5-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="725b5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="725b5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="725b5-135">Response</span></span>

<span data-ttu-id="725b5-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="725b5-136">The following is an example of the response.</span></span>

> <span data-ttu-id="725b5-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="725b5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
      "status": "Active",
      "machineName": "server1.local1.contoso.com",
      "externalIp": "153.69.23.122",
      "agentGroups": [
        {
          "id": "2d55ed41-1619-4848-92bb-0576d3038682",
          "displayName": "Group 1"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agentGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
