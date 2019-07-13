---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387c0a934b2b2ae005248b0fd1c0111da00387d4
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639084"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="10bd7-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="10bd7-103">Get subscribedSku</span></span>

<span data-ttu-id="10bd7-104">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="10bd7-104">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="10bd7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="10bd7-105">Permissions</span></span>
<span data-ttu-id="10bd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10bd7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10bd7-108">Permission type</span></span>      | <span data-ttu-id="10bd7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10bd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bd7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10bd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10bd7-111">Organization. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="10bd7-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10bd7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10bd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bd7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bd7-113">Not supported.</span></span>    |
|<span data-ttu-id="10bd7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bd7-114">Application</span></span> | <span data-ttu-id="10bd7-115">Organization. Read. All, Directory. Read. All, Organization. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="10bd7-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10bd7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10bd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10bd7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10bd7-117">Optional query parameters</span></span>
<span data-ttu-id="10bd7-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="10bd7-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="10bd7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10bd7-119">Request headers</span></span>

| <span data-ttu-id="10bd7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="10bd7-120">Name</span></span>       | <span data-ttu-id="10bd7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="10bd7-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="10bd7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10bd7-122">Authorization</span></span>  | <span data-ttu-id="10bd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10bd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10bd7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10bd7-125">Request body</span></span>
<span data-ttu-id="10bd7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10bd7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10bd7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bd7-127">Response</span></span>

<span data-ttu-id="10bd7-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10bd7-128">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10bd7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10bd7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10bd7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10bd7-130">Request</span></span>
<span data-ttu-id="10bd7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10bd7-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="10bd7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="10bd7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10bd7-133">C#</span><span class="sxs-lookup"><span data-stu-id="10bd7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10bd7-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="10bd7-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10bd7-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="10bd7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10bd7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bd7-136">Response</span></span>
<span data-ttu-id="10bd7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10bd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
    "capabilityStatus": "Enabled",
    "consumedUnits": 14,
    "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
    "prepaidUnits": {
        "enabled": 25,
        "suspended": 0,
        "warning": 0
    },
    "servicePlans": [
        {
            "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
            "servicePlanName": "ADALLOM_S_O365",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
