---
title: Obter publishedResource
description: Recupere as propriedades e os relacionamentos de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1555adb5603d734534437037a52527313eaeac24
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199762"
---
# <a name="get-publishedresource"></a><span data-ttu-id="3a9ba-103">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="3a9ba-103">Get publishedResource</span></span>

<span data-ttu-id="3a9ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a9ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a9ba-105">Recupere as propriedades e os relacionamentos do objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="3a9ba-105">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a9ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a9ba-106">Permissions</span></span>

<span data-ttu-id="3a9ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a9ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a9ba-109">Permission type</span></span>                        | <span data-ttu-id="3a9ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a9ba-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="3a9ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a9ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a9ba-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9ba-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="3a9ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a9ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a9ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-114">Not supported.</span></span> |
| <span data-ttu-id="3a9ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a9ba-115">Application</span></span>                            | <span data-ttu-id="3a9ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a9ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a9ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a9ba-118">Optional query parameters</span></span>

<span data-ttu-id="3a9ba-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a9ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ba-120">Request headers</span></span>

| <span data-ttu-id="3a9ba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3a9ba-121">Name</span></span>      |<span data-ttu-id="3a9ba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a9ba-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a9ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a9ba-123">Authorization</span></span> | <span data-ttu-id="3a9ba-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="3a9ba-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a9ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ba-125">Request body</span></span>

<span data-ttu-id="3a9ba-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a9ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9ba-127">Response</span></span>

<span data-ttu-id="3a9ba-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [publishedResource](../resources/publishedresource.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-128">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a9ba-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a9ba-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a9ba-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a9ba-130">Request</span></span>

<span data-ttu-id="3a9ba-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a9ba-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9ba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="3a9ba-133">C#</span><span class="sxs-lookup"><span data-stu-id="3a9ba-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a9ba-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a9ba-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a9ba-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a9ba-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a9ba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a9ba-136">Response</span></span>

<span data-ttu-id="3a9ba-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-137">The following is an example of the response.</span></span>

> <span data-ttu-id="3a9ba-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a9ba-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
