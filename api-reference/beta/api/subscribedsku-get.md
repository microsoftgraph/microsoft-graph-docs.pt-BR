---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8cdcbf9a3de784d3158d1393329f3df9e4262d1f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457132"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="6a296-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="6a296-103">Get subscribedSku</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a296-104">Recupere uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="6a296-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a296-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a296-105">Permissions</span></span>
<span data-ttu-id="6a296-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a296-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a296-108">Permission type</span></span>      | <span data-ttu-id="6a296-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a296-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a296-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a296-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a296-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a296-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a296-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a296-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a296-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a296-113">Not supported.</span></span>    |
|<span data-ttu-id="6a296-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a296-114">Application</span></span> | <span data-ttu-id="6a296-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a296-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a296-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a296-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a296-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a296-117">Optional query parameters</span></span>
<span data-ttu-id="6a296-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a296-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a296-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a296-119">Request headers</span></span>
| <span data-ttu-id="6a296-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6a296-120">Name</span></span>       | <span data-ttu-id="6a296-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a296-121">Type</span></span> | <span data-ttu-id="6a296-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a296-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a296-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a296-123">Authorization</span></span>  | <span data-ttu-id="6a296-124">string</span><span class="sxs-lookup"><span data-stu-id="6a296-124">string</span></span>  | <span data-ttu-id="6a296-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a296-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a296-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a296-127">Request body</span></span>
<span data-ttu-id="6a296-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a296-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a296-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a296-129">Response</span></span>

<span data-ttu-id="6a296-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a296-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a296-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a296-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a296-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a296-132">Request</span></span>
<span data-ttu-id="6a296-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a296-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a296-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a296-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a296-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a296-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a296-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a296-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a296-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a296-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a296-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a296-138">Response</span></span>
<span data-ttu-id="6a296-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a296-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
