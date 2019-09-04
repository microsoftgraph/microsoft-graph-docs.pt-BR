---
title: Obter onPremisesAgent
description: Recupere as propriedades e os relacionamentos de um objeto onPremisesAgent.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba647ac06afdc91b812cf87b962013f5572320e1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726008"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="085de-103">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="085de-103">Get onPremisesAgent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="085de-104">Recupere as propriedades e os relacionamentos de um objeto [onPremisesAgent](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="085de-104">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="085de-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="085de-105">Permissions</span></span>

<span data-ttu-id="085de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="085de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="085de-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="085de-108">Permission type</span></span>                        | <span data-ttu-id="085de-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="085de-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="085de-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="085de-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="085de-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="085de-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="085de-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="085de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="085de-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="085de-113">Not supported.</span></span> |
| <span data-ttu-id="085de-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="085de-114">Application</span></span>                            | <span data-ttu-id="085de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="085de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="085de-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="085de-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="085de-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="085de-117">Optional query parameters</span></span>

<span data-ttu-id="085de-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="085de-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="085de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="085de-119">Request headers</span></span>

| <span data-ttu-id="085de-120">Nome</span><span class="sxs-lookup"><span data-stu-id="085de-120">Name</span></span>      |<span data-ttu-id="085de-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="085de-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="085de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="085de-122">Authorization</span></span> | <span data-ttu-id="085de-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="085de-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="085de-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="085de-124">Request body</span></span>

<span data-ttu-id="085de-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="085de-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="085de-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="085de-126">Response</span></span>

<span data-ttu-id="085de-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onPremisesAgent](../resources/onpremisesagent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="085de-127">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="085de-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="085de-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="085de-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="085de-129">Request</span></span>

<span data-ttu-id="085de-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="085de-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="085de-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="085de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="085de-132">C#</span><span class="sxs-lookup"><span data-stu-id="085de-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="085de-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="085de-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="085de-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="085de-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="085de-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="085de-135">Response</span></span>

<span data-ttu-id="085de-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="085de-136">The following is an example of the response.</span></span>

> <span data-ttu-id="085de-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="085de-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
