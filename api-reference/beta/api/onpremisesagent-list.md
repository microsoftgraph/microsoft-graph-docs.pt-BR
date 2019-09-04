---
title: Listar onPremisesAgents
description: Recupere uma lista de onPremisesAgents.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e8b80c5333f33b25f7bc86df454d0be9e826a131
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723823"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="f8cdb-103">Listar onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="f8cdb-103">List onPremisesAgents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8cdb-104">Recupere uma lista de objetos [onPremisesAgent](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="f8cdb-104">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8cdb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8cdb-105">Permissions</span></span>

<span data-ttu-id="f8cdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8cdb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8cdb-108">Permission type</span></span>                        | <span data-ttu-id="f8cdb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8cdb-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8cdb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8cdb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8cdb-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8cdb-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f8cdb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8cdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8cdb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-113">Not supported.</span></span> |
| <span data-ttu-id="f8cdb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8cdb-114">Application</span></span>                            | <span data-ttu-id="f8cdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8cdb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8cdb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8cdb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8cdb-117">Optional query parameters</span></span>

<span data-ttu-id="f8cdb-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8cdb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cdb-119">Request headers</span></span>

| <span data-ttu-id="f8cdb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f8cdb-120">Name</span></span>      |<span data-ttu-id="f8cdb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8cdb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8cdb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8cdb-122">Authorization</span></span> | <span data-ttu-id="f8cdb-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f8cdb-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8cdb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cdb-124">Request body</span></span>

<span data-ttu-id="f8cdb-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8cdb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8cdb-126">Response</span></span>

<span data-ttu-id="f8cdb-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-127">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8cdb-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8cdb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8cdb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cdb-129">Request</span></span>

<span data-ttu-id="f8cdb-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f8cdb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8cdb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8cdb-132">C#</span><span class="sxs-lookup"><span data-stu-id="f8cdb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8cdb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8cdb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8cdb-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f8cdb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8cdb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8cdb-135">Response</span></span>

<span data-ttu-id="f8cdb-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f8cdb-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8cdb-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
