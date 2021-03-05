---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a24383651264a66cc36f61bc87c021892b7401df
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441673"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="fac95-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="fac95-103">Get subscribedSku</span></span>

<span data-ttu-id="fac95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fac95-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fac95-105">Obter uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="fac95-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="fac95-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fac95-106">Permissions</span></span>
<span data-ttu-id="fac95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fac95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fac95-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fac95-109">Permission type</span></span>      | <span data-ttu-id="fac95-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fac95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fac95-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fac95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fac95-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fac95-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fac95-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fac95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fac95-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fac95-114">Not supported.</span></span>    |
|<span data-ttu-id="fac95-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fac95-115">Application</span></span> | <span data-ttu-id="fac95-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fac95-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fac95-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fac95-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fac95-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fac95-118">Optional query parameters</span></span>
<span data-ttu-id="fac95-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="fac95-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fac95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fac95-120">Request headers</span></span>

| <span data-ttu-id="fac95-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fac95-121">Name</span></span>       | <span data-ttu-id="fac95-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fac95-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="fac95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fac95-123">Authorization</span></span>  | <span data-ttu-id="fac95-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fac95-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fac95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fac95-126">Request body</span></span>
<span data-ttu-id="fac95-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fac95-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fac95-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac95-128">Response</span></span>

<span data-ttu-id="fac95-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fac95-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fac95-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fac95-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fac95-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fac95-131">Request</span></span>
<span data-ttu-id="fac95-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fac95-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fac95-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fac95-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="fac95-134">C#</span><span class="sxs-lookup"><span data-stu-id="fac95-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fac95-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fac95-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fac95-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fac95-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fac95-137">Java</span><span class="sxs-lookup"><span data-stu-id="fac95-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedsku-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fac95-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fac95-138">Response</span></span>
<span data-ttu-id="fac95-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fac95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
