---
title: Obter onPremisesAgentGroup
description: Recupere as propriedades e os relacionamentos de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c7b46c9a7183ddb9706212f6afb73bbf01caa1
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199932"
---
# <a name="get-onpremisesagentgroup"></a><span data-ttu-id="b2959-103">Obter onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="b2959-103">Get onPremisesAgentGroup</span></span>

<span data-ttu-id="b2959-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2959-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2959-105">Recupere as propriedades e os relacionamentos de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b2959-105">Retrieve the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2959-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2959-106">Permissions</span></span>

<span data-ttu-id="b2959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2959-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2959-109">Permission type</span></span>                        | <span data-ttu-id="b2959-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2959-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2959-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2959-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2959-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2959-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b2959-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2959-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2959-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2959-114">Not supported.</span></span> |
| <span data-ttu-id="b2959-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2959-115">Application</span></span>                            | <span data-ttu-id="b2959-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2959-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2959-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2959-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2959-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b2959-118">Optional query parameters</span></span>

<span data-ttu-id="b2959-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b2959-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2959-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2959-120">Request headers</span></span>

| <span data-ttu-id="b2959-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b2959-121">Name</span></span>      |<span data-ttu-id="b2959-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2959-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2959-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2959-123">Authorization</span></span> | <span data-ttu-id="b2959-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b2959-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2959-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2959-125">Request body</span></span>

<span data-ttu-id="b2959-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2959-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2959-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2959-127">Response</span></span>

<span data-ttu-id="b2959-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2959-128">If successful, this method returns a `200 OK` response code and the requested [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2959-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b2959-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2959-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2959-130">Request</span></span>

<span data-ttu-id="b2959-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2959-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2959-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2959-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagentgroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/?$expand=publishedResources,agents
```
# <a name="c"></a>[<span data-ttu-id="b2959-133">C#</span><span class="sxs-lookup"><span data-stu-id="b2959-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2959-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2959-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2959-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2959-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2959-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2959-136">Response</span></span>

<span data-ttu-id="b2959-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2959-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b2959-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2959-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
            "displayName": "Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
