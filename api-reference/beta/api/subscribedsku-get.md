---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5283efcd46c9c78d1e500dafd45dc590d7399d85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43318799"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="87982-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="87982-103">Get subscribedSku</span></span>

<span data-ttu-id="87982-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87982-105">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="87982-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="87982-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87982-106">Permissions</span></span>
<span data-ttu-id="87982-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87982-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87982-109">Permission type</span></span>      | <span data-ttu-id="87982-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87982-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87982-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87982-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87982-112">Organization. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="87982-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87982-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87982-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87982-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87982-114">Not supported.</span></span>    |
|<span data-ttu-id="87982-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87982-115">Application</span></span> | <span data-ttu-id="87982-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87982-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87982-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87982-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87982-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87982-118">Optional query parameters</span></span>
<span data-ttu-id="87982-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87982-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87982-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87982-120">Request headers</span></span>

| <span data-ttu-id="87982-121">Nome</span><span class="sxs-lookup"><span data-stu-id="87982-121">Name</span></span>       | <span data-ttu-id="87982-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87982-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="87982-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87982-123">Authorization</span></span>  | <span data-ttu-id="87982-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87982-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87982-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87982-126">Request body</span></span>
<span data-ttu-id="87982-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87982-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87982-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="87982-128">Response</span></span>

<span data-ttu-id="87982-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87982-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87982-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87982-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87982-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87982-131">Request</span></span>
<span data-ttu-id="87982-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87982-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87982-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="87982-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="87982-134">C#</span><span class="sxs-lookup"><span data-stu-id="87982-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87982-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87982-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87982-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87982-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87982-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="87982-137">Response</span></span>
<span data-ttu-id="87982-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87982-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

{
  "capabilityStatus": "capabilityStatus-value",
  "consumedUnits": 99,
  "prepaidUnits": {
    "enabled": 99,
    "suspended": 99,
    "warning": 99
  },
  "servicePlans": [
    {
      "servicePlanId": "servicePlanId-value",
      "servicePlanName": "servicePlanName-value",
      "provisioningStatus": "provisioningStatus-value",
      "appliesTo": "appliesTo-value"
    }
  ],
  "skuId": "skuId-value",
  "skuPartNumber": "skuPartNumber-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
