---
title: Listar onPremisesAgentGroups
description: Recupere uma lista de objetos onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53409381e117c0c93d4626642397f1952fabc864
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878362"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="6a87c-103">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="6a87c-103">List onPremisesAgentGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a87c-104">Recupere uma lista de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6a87c-104">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a87c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a87c-105">Permissions</span></span>

<span data-ttu-id="6a87c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a87c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a87c-108">Permission type</span></span>                        | <span data-ttu-id="6a87c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a87c-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a87c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a87c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a87c-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a87c-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6a87c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a87c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a87c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a87c-113">Not supported.</span></span> |
| <span data-ttu-id="6a87c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a87c-114">Application</span></span>                            | <span data-ttu-id="6a87c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a87c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a87c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a87c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a87c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a87c-117">Optional query parameters</span></span>

<span data-ttu-id="6a87c-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a87c-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a87c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a87c-119">Request headers</span></span>

| <span data-ttu-id="6a87c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6a87c-120">Name</span></span>      |<span data-ttu-id="6a87c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a87c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a87c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a87c-122">Authorization</span></span> | <span data-ttu-id="6a87c-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6a87c-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a87c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a87c-124">Request body</span></span>

<span data-ttu-id="6a87c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a87c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a87c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a87c-126">Response</span></span>

<span data-ttu-id="6a87c-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a87c-127">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a87c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a87c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a87c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a87c-129">Request</span></span>

<span data-ttu-id="6a87c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a87c-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a87c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a87c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a87c-132">C#</span><span class="sxs-lookup"><span data-stu-id="6a87c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a87c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a87c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a87c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a87c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a87c-135">Java</span><span class="sxs-lookup"><span data-stu-id="6a87c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agentgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a87c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a87c-136">Response</span></span>

<span data-ttu-id="6a87c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a87c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6a87c-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a87c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
