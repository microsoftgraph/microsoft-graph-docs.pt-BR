---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf9a8213b4beaf62208b4857584da981367b6fcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520801"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="ad145-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ad145-103">Get subscribedSku</span></span>
<span data-ttu-id="ad145-104">Recupere uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="ad145-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad145-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad145-105">Permissions</span></span>
<span data-ttu-id="ad145-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad145-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad145-108">Permission type</span></span>      | <span data-ttu-id="ad145-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad145-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad145-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad145-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad145-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad145-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad145-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad145-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad145-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad145-113">Not supported.</span></span>    |
|<span data-ttu-id="ad145-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad145-114">Application</span></span> | <span data-ttu-id="ad145-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad145-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad145-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad145-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad145-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad145-117">Optional query parameters</span></span>
<span data-ttu-id="ad145-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="ad145-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad145-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad145-119">Request headers</span></span>
| <span data-ttu-id="ad145-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ad145-120">Name</span></span>       | <span data-ttu-id="ad145-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad145-121">Type</span></span> | <span data-ttu-id="ad145-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad145-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ad145-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad145-123">Authorization</span></span>  | <span data-ttu-id="ad145-124">string</span><span class="sxs-lookup"><span data-stu-id="ad145-124">string</span></span>  | <span data-ttu-id="ad145-p102">&lt;Token&gt; de portador. *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="ad145-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad145-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad145-127">Request body</span></span>
<span data-ttu-id="ad145-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad145-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad145-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad145-129">Response</span></span>

<span data-ttu-id="ad145-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad145-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad145-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad145-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad145-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad145-132">Request</span></span>
<span data-ttu-id="ad145-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad145-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="ad145-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad145-134">Response</span></span>
<span data-ttu-id="ad145-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad145-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
