---
title: Listar publishedResources
description: Recupere uma lista de objetos publishedResource.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7670583a4614dac3466fbb21ede09b7aea03f73c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055173"
---
# <a name="list-publishedresources"></a><span data-ttu-id="7108c-103">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="7108c-103">List publishedResources</span></span>

<span data-ttu-id="7108c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7108c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7108c-105">Recupere uma lista de [objetos publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="7108c-105">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7108c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7108c-106">Permissions</span></span>

<span data-ttu-id="7108c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7108c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7108c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7108c-109">Permission type</span></span>                        | <span data-ttu-id="7108c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7108c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="7108c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7108c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7108c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7108c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7108c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7108c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7108c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7108c-114">Not supported.</span></span> |
| <span data-ttu-id="7108c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7108c-115">Application</span></span>                            | <span data-ttu-id="7108c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7108c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7108c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7108c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7108c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7108c-118">Optional query parameters</span></span>

<span data-ttu-id="7108c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7108c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7108c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7108c-120">Request headers</span></span>

| <span data-ttu-id="7108c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7108c-121">Name</span></span>      |<span data-ttu-id="7108c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7108c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7108c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7108c-123">Authorization</span></span> | <span data-ttu-id="7108c-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="7108c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7108c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7108c-125">Request body</span></span>

<span data-ttu-id="7108c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7108c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7108c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7108c-127">Response</span></span>

<span data-ttu-id="7108c-128">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7108c-128">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7108c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7108c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7108c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7108c-130">Request</span></span>

<span data-ttu-id="7108c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7108c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7108c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7108c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="7108c-133">C#</span><span class="sxs-lookup"><span data-stu-id="7108c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7108c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7108c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7108c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7108c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7108c-136">Java</span><span class="sxs-lookup"><span data-stu-id="7108c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7108c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7108c-137">Response</span></span>

<span data-ttu-id="7108c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7108c-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7108c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7108c-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List publishedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



