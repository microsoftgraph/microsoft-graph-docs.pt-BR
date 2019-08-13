---
title: Obter publishedResource
description: Recupere as propriedades e os relacionamentos de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 053d522d8bc9f51d6c53cf0f7c0159da46fdd876
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309241"
---
# <a name="get-publishedresource"></a><span data-ttu-id="61f58-103">Obter publishedResource</span><span class="sxs-lookup"><span data-stu-id="61f58-103">Get publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61f58-104">Recupere as propriedades e os relacionamentos do objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="61f58-104">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61f58-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="61f58-105">Permissions</span></span>

<span data-ttu-id="61f58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61f58-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61f58-108">Permission type</span></span>                        | <span data-ttu-id="61f58-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61f58-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="61f58-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61f58-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="61f58-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="61f58-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="61f58-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61f58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61f58-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61f58-113">Not supported.</span></span> |
| <span data-ttu-id="61f58-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61f58-114">Application</span></span>                            | <span data-ttu-id="61f58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61f58-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61f58-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61f58-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61f58-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61f58-117">Optional query parameters</span></span>

<span data-ttu-id="61f58-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61f58-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61f58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61f58-119">Request headers</span></span>

| <span data-ttu-id="61f58-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61f58-120">Name</span></span>      |<span data-ttu-id="61f58-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="61f58-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61f58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61f58-122">Authorization</span></span> | <span data-ttu-id="61f58-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="61f58-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="61f58-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61f58-124">Request body</span></span>

<span data-ttu-id="61f58-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61f58-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61f58-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="61f58-126">Response</span></span>

<span data-ttu-id="61f58-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [publishedResource](../resources/publishedresource.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61f58-127">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61f58-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61f58-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61f58-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61f58-129">Request</span></span>

<span data-ttu-id="61f58-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61f58-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="61f58-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="61f58-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61f58-132">C#</span><span class="sxs-lookup"><span data-stu-id="61f58-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61f58-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61f58-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61f58-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="61f58-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="61f58-135">Java</span><span class="sxs-lookup"><span data-stu-id="61f58-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61f58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="61f58-136">Response</span></span>

<span data-ttu-id="61f58-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61f58-137">The following is an example of the response.</span></span>

> <span data-ttu-id="61f58-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61f58-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
