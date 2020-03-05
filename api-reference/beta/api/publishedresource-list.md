---
title: Listar publishedResources
description: Recupere uma lista de objetos publishedResource.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 370a13906e931e20eaea1a4dbd2fb1bc17a2ea50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454840"
---
# <a name="list-publishedresources"></a><span data-ttu-id="b7be5-103">Listar publishedResources</span><span class="sxs-lookup"><span data-stu-id="b7be5-103">List publishedResources</span></span>

<span data-ttu-id="b7be5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b7be5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7be5-105">Recupere uma lista de objetos [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="b7be5-105">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7be5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7be5-106">Permissions</span></span>

<span data-ttu-id="b7be5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7be5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7be5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7be5-109">Permission type</span></span>                        | <span data-ttu-id="b7be5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7be5-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b7be5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7be5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7be5-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7be5-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b7be5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7be5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7be5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7be5-114">Not supported.</span></span> |
| <span data-ttu-id="b7be5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7be5-115">Application</span></span>                            | <span data-ttu-id="b7be5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7be5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7be5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7be5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7be5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7be5-118">Optional query parameters</span></span>

<span data-ttu-id="b7be5-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7be5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7be5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7be5-120">Request headers</span></span>

| <span data-ttu-id="b7be5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b7be5-121">Name</span></span>      |<span data-ttu-id="b7be5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7be5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7be5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7be5-123">Authorization</span></span> | <span data-ttu-id="b7be5-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b7be5-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7be5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7be5-125">Request body</span></span>

<span data-ttu-id="b7be5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7be5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7be5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7be5-127">Response</span></span>

<span data-ttu-id="b7be5-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7be5-128">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7be5-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7be5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7be5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7be5-130">Request</span></span>

<span data-ttu-id="b7be5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7be5-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7be5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7be5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="b7be5-133">C#</span><span class="sxs-lookup"><span data-stu-id="b7be5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7be5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7be5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7be5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7be5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7be5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7be5-136">Response</span></span>

<span data-ttu-id="b7be5-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7be5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b7be5-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7be5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
