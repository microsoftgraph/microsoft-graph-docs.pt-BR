---
title: Atualizar clientes
description: Atualiza um objeto do cliente no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e19c24cd453a5702e64019e6fb96903786d41a19
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045625"
---
# <a name="update-customers"></a><span data-ttu-id="02ba2-103">Atualizar clientes</span><span class="sxs-lookup"><span data-stu-id="02ba2-103">Update customers</span></span>

<span data-ttu-id="02ba2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02ba2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02ba2-105">Atualize as propriedades de um objeto do cliente para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="02ba2-105">Update the properties of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="02ba2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02ba2-106">Permissions</span></span>
<span data-ttu-id="02ba2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ba2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02ba2-109">Permission type</span></span> |<span data-ttu-id="02ba2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02ba2-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="02ba2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02ba2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02ba2-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ba2-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="02ba2-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="02ba2-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="02ba2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02ba2-114">Not supported.</span></span>|
|<span data-ttu-id="02ba2-115">Application</span><span class="sxs-lookup"><span data-stu-id="02ba2-115">Application</span></span>|<span data-ttu-id="02ba2-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ba2-116">Financials.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="02ba2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02ba2-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02ba2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02ba2-118">Optional query parameters</span></span>
<span data-ttu-id="02ba2-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02ba2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02ba2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02ba2-120">Request headers</span></span>
|<span data-ttu-id="02ba2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02ba2-121">Header</span></span>         |<span data-ttu-id="02ba2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02ba2-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="02ba2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02ba2-123">Authorization</span></span>  |<span data-ttu-id="02ba2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02ba2-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="02ba2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02ba2-126">Content-Type</span></span>   |<span data-ttu-id="02ba2-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="02ba2-127">application/json.</span></span>         |
|<span data-ttu-id="02ba2-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="02ba2-128">If-Match</span></span>       |<span data-ttu-id="02ba2-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02ba2-129">Required.</span></span> <span data-ttu-id="02ba2-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos clientes **,** os clientes **não** serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="02ba2-130">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02ba2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02ba2-131">Request body</span></span>
<span data-ttu-id="02ba2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02ba2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="02ba2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="02ba2-135">Response</span></span>
<span data-ttu-id="02ba2-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto **de clientes** atualizados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ba2-136">If successful, this method returns a `200 OK` response code and an updated **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02ba2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02ba2-137">Example</span></span>

<span data-ttu-id="02ba2-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="02ba2-138">**Request**</span></span>

<span data-ttu-id="02ba2-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02ba2-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
Content-type: application/json

{
  "displayName": "Coho Winery Inc.",
  "phoneNumber": "(555) 555-1234"
}
```

<span data-ttu-id="02ba2-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="02ba2-140">**Response**</span></span>

<span data-ttu-id="02ba2-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ba2-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="02ba2-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02ba2-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery Inc.",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "(555) 555-1234"
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethod-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```




