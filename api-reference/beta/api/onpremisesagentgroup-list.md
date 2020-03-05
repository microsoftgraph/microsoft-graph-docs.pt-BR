---
title: Listar onPremisesAgentGroups
description: Recupere uma lista de objetos onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84177ae4054071fb60b6d323d034a6076eb8d9ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456457"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="c8ced-103">Listar onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="c8ced-103">List onPremisesAgentGroups</span></span>

<span data-ttu-id="c8ced-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c8ced-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8ced-105">Recupere uma lista de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c8ced-105">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8ced-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8ced-106">Permissions</span></span>

<span data-ttu-id="c8ced-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8ced-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8ced-109">Permission type</span></span>                        | <span data-ttu-id="c8ced-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8ced-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8ced-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8ced-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8ced-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ced-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="c8ced-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8ced-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ced-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8ced-114">Not supported.</span></span> |
| <span data-ttu-id="c8ced-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8ced-115">Application</span></span>                            | <span data-ttu-id="c8ced-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8ced-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8ced-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ced-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8ced-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8ced-118">Optional query parameters</span></span>

<span data-ttu-id="c8ced-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ced-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8ced-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ced-120">Request headers</span></span>

| <span data-ttu-id="c8ced-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c8ced-121">Name</span></span>      |<span data-ttu-id="c8ced-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8ced-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8ced-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8ced-123">Authorization</span></span> | <span data-ttu-id="c8ced-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c8ced-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8ced-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ced-125">Request body</span></span>

<span data-ttu-id="c8ced-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8ced-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8ced-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ced-127">Response</span></span>

<span data-ttu-id="c8ced-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ced-128">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8ced-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c8ced-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8ced-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ced-130">Request</span></span>

<span data-ttu-id="c8ced-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8ced-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8ced-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ced-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="c"></a>[<span data-ttu-id="c8ced-133">C#</span><span class="sxs-lookup"><span data-stu-id="c8ced-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8ced-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8ced-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8ced-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8ced-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8ced-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ced-136">Response</span></span>

<span data-ttu-id="c8ced-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ced-137">The following is an example of the response.</span></span>

> <span data-ttu-id="c8ced-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8ced-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
