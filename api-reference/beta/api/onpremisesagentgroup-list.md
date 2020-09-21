---
title: Listar onPremisesAgentGroups
description: Recupere uma lista de objetos onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02374b55c5d1905c26675ea5419dce3115e3c4c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969498"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="732b3-103">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="732b3-103">List onPremisesAgentGroups</span></span>

<span data-ttu-id="732b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="732b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="732b3-105">Recupere uma lista de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="732b3-105">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="732b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="732b3-106">Permissions</span></span>

<span data-ttu-id="732b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="732b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="732b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="732b3-109">Permission type</span></span>                        | <span data-ttu-id="732b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="732b3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="732b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="732b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="732b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="732b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="732b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="732b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="732b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="732b3-114">Not supported.</span></span> |
| <span data-ttu-id="732b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="732b3-115">Application</span></span>                            | <span data-ttu-id="732b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="732b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="732b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="732b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="732b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="732b3-118">Optional query parameters</span></span>

<span data-ttu-id="732b3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="732b3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="732b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="732b3-120">Request headers</span></span>

| <span data-ttu-id="732b3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="732b3-121">Name</span></span>      |<span data-ttu-id="732b3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="732b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="732b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="732b3-123">Authorization</span></span> | <span data-ttu-id="732b3-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="732b3-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="732b3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="732b3-125">Request body</span></span>

<span data-ttu-id="732b3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="732b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="732b3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="732b3-127">Response</span></span>

<span data-ttu-id="732b3-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="732b3-128">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="732b3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="732b3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="732b3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="732b3-130">Request</span></span>

<span data-ttu-id="732b3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="732b3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="732b3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="732b3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="c"></a>[<span data-ttu-id="732b3-133">C#</span><span class="sxs-lookup"><span data-stu-id="732b3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="732b3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="732b3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="732b3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="732b3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="732b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="732b3-136">Response</span></span>

<span data-ttu-id="732b3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="732b3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="732b3-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="732b3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1",
            "publishingType": "provisioning",
            "isDefault": false,
            "agents": [
                 {
                    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
                    "status": "Active"
                 }
            ],
            "publishedResources": [
                {
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
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
  "description": "List agents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


