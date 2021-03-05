---
title: Listar subscribedSkus
description: Recupere a lista de assinaturas comerciais que uma organização adquiriu.
localization_priority: Priority
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0e1d403e4930c9edcf48dd7c008fd95c9d3fbe61
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442534"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="d0139-103">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="d0139-103">List subscribedSkus</span></span>

<span data-ttu-id="d0139-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0139-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0139-105">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="d0139-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0139-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0139-106">Permissions</span></span>
<span data-ttu-id="d0139-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d0139-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0139-109">Permission type</span></span>      | <span data-ttu-id="d0139-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0139-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0139-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0139-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0139-112">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0139-112">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0139-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0139-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0139-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0139-114">Not supported.</span></span>    |
|<span data-ttu-id="d0139-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0139-115">Application</span></span> | <span data-ttu-id="d0139-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0139-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0139-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0139-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0139-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0139-118">Optional query parameters</span></span>
<span data-ttu-id="d0139-119">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="d0139-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0139-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0139-120">Request headers</span></span>

| <span data-ttu-id="d0139-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d0139-121">Name</span></span>       | <span data-ttu-id="d0139-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0139-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="d0139-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0139-123">Authorization</span></span>  | <span data-ttu-id="d0139-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0139-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0139-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0139-126">Request body</span></span>
<span data-ttu-id="d0139-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0139-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0139-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0139-128">Response</span></span>

<span data-ttu-id="d0139-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0139-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0139-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0139-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0139-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0139-131">Request</span></span>
<span data-ttu-id="d0139-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0139-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0139-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0139-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="d0139-134">C#</span><span class="sxs-lookup"><span data-stu-id="d0139-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0139-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0139-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0139-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0139-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0139-137">Java</span><span class="sxs-lookup"><span data-stu-id="d0139-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0139-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0139-138">Response</span></span>
<span data-ttu-id="d0139-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0139-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
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
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
