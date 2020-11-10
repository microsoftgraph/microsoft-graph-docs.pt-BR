---
title: Listar onPremisesAgents
description: Recupere uma lista de onPremisesAgents.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9690d9a3616d581e7cac64865f9a1ca45c7d064
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975646"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="73b91-103">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="73b91-103">List onPremisesAgents</span></span>

<span data-ttu-id="73b91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b91-105">Recupere uma lista de objetos [onPremisesAgent](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="73b91-105">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b91-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="73b91-106">Permissions</span></span>

<span data-ttu-id="73b91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73b91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73b91-109">Permission type</span></span>                        | <span data-ttu-id="73b91-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73b91-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b91-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73b91-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="73b91-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b91-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="73b91-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73b91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b91-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73b91-114">Not supported.</span></span> |
| <span data-ttu-id="73b91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73b91-115">Application</span></span>                            | <span data-ttu-id="73b91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73b91-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73b91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73b91-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73b91-118">Optional query parameters</span></span>

<span data-ttu-id="73b91-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73b91-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73b91-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73b91-120">Request headers</span></span>

| <span data-ttu-id="73b91-121">Nome</span><span class="sxs-lookup"><span data-stu-id="73b91-121">Name</span></span>      |<span data-ttu-id="73b91-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="73b91-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73b91-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73b91-123">Authorization</span></span> | <span data-ttu-id="73b91-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="73b91-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73b91-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73b91-125">Request body</span></span>

<span data-ttu-id="73b91-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73b91-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b91-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="73b91-127">Response</span></span>

<span data-ttu-id="73b91-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73b91-128">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73b91-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73b91-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73b91-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73b91-130">Request</span></span>

<span data-ttu-id="73b91-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73b91-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73b91-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="73b91-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="73b91-133">C#</span><span class="sxs-lookup"><span data-stu-id="73b91-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73b91-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73b91-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73b91-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73b91-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73b91-136">Java</span><span class="sxs-lookup"><span data-stu-id="73b91-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73b91-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="73b91-137">Response</span></span>

<span data-ttu-id="73b91-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73b91-138">The following is an example of the response.</span></span>

> <span data-ttu-id="73b91-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73b91-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


