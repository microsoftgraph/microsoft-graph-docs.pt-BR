---
title: Obter publishedResource
description: Recupere as propriedades e os relacionamentos de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: def49c80a2c1529d02b643bdc6f97b8fdd5d959d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454858"
---
# <a name="get-publishedresource"></a><span data-ttu-id="383b3-103">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="383b3-103">Get publishedResource</span></span>

<span data-ttu-id="383b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="383b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="383b3-105">Recupere as propriedades e os relacionamentos do objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="383b3-105">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="383b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="383b3-106">Permissions</span></span>

<span data-ttu-id="383b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="383b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="383b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="383b3-109">Permission type</span></span>                        | <span data-ttu-id="383b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="383b3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="383b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="383b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="383b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="383b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="383b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="383b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="383b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="383b3-114">Not supported.</span></span> |
| <span data-ttu-id="383b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="383b3-115">Application</span></span>                            | <span data-ttu-id="383b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="383b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="383b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="383b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="383b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="383b3-118">Optional query parameters</span></span>

<span data-ttu-id="383b3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="383b3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="383b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="383b3-120">Request headers</span></span>

| <span data-ttu-id="383b3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="383b3-121">Name</span></span>      |<span data-ttu-id="383b3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="383b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="383b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="383b3-123">Authorization</span></span> | <span data-ttu-id="383b3-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="383b3-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="383b3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="383b3-125">Request body</span></span>

<span data-ttu-id="383b3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="383b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="383b3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="383b3-127">Response</span></span>

<span data-ttu-id="383b3-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [publishedResource](../resources/publishedresource.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="383b3-128">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="383b3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="383b3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="383b3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="383b3-130">Request</span></span>

<span data-ttu-id="383b3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="383b3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="383b3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="383b3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="383b3-133">C#</span><span class="sxs-lookup"><span data-stu-id="383b3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="383b3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="383b3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="383b3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="383b3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="383b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="383b3-136">Response</span></span>

<span data-ttu-id="383b3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="383b3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="383b3-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="383b3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "publishingType": "provisioning",
    "displayName": "Demo provisioning",
    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
    "resourceName": "domain1.contoso.com",
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
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
