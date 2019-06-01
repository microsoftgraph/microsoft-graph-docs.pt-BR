---
title: Obter subscribedSku
description: Recupere uma assinatura comercial específica que uma organização adquiriu.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c780ef1460c98e558eee03ae8535b150b25c99b8
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657452"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="97042-103">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="97042-103">Get subscribedSku</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97042-104">Recupere uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="97042-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="97042-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97042-105">Permissions</span></span>
<span data-ttu-id="97042-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="97042-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97042-108">Permission type</span></span>      | <span data-ttu-id="97042-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97042-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97042-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97042-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97042-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97042-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97042-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97042-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97042-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97042-113">Not supported.</span></span>    |
|<span data-ttu-id="97042-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97042-114">Application</span></span> | <span data-ttu-id="97042-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97042-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97042-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97042-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97042-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97042-117">Optional query parameters</span></span>
<span data-ttu-id="97042-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97042-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97042-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97042-119">Request headers</span></span>
| <span data-ttu-id="97042-120">Nome</span><span class="sxs-lookup"><span data-stu-id="97042-120">Name</span></span>       | <span data-ttu-id="97042-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="97042-121">Type</span></span> | <span data-ttu-id="97042-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="97042-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97042-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97042-123">Authorization</span></span>  | <span data-ttu-id="97042-124">string</span><span class="sxs-lookup"><span data-stu-id="97042-124">string</span></span>  | <span data-ttu-id="97042-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97042-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97042-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97042-127">Request body</span></span>
<span data-ttu-id="97042-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97042-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97042-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="97042-129">Response</span></span>

<span data-ttu-id="97042-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97042-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97042-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97042-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97042-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97042-132">Request</span></span>
<span data-ttu-id="97042-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97042-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="97042-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="97042-134">Response</span></span>
<span data-ttu-id="97042-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97042-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="97042-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="97042-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="97042-139">C#</span><span class="sxs-lookup"><span data-stu-id="97042-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97042-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="97042-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
