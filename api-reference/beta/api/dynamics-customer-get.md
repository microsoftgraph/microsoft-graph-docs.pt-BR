---
title: Obter clientes
description: Obtém um objeto do cliente no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: df34248e6977752504f1f1c8f0997fbc0fa8f434
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045632"
---
# <a name="get-customers"></a><span data-ttu-id="89ecc-103">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="89ecc-103">Get customers</span></span>

<span data-ttu-id="89ecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89ecc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89ecc-105">Recupere as propriedades e as relações de um objeto do cliente para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="89ecc-105">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ecc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89ecc-106">Permissions</span></span>
<span data-ttu-id="89ecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ecc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ecc-109">Permission type</span></span> |<span data-ttu-id="89ecc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89ecc-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="89ecc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ecc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89ecc-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ecc-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="89ecc-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="89ecc-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="89ecc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ecc-114">Not supported.</span></span>|
|<span data-ttu-id="89ecc-115">Application</span><span class="sxs-lookup"><span data-stu-id="89ecc-115">Application</span></span>|<span data-ttu-id="89ecc-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ecc-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ecc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ecc-117">HTTP request</span></span>
```
GET /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89ecc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89ecc-118">Optional query parameters</span></span>
<span data-ttu-id="89ecc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89ecc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ecc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ecc-120">Request headers</span></span>
|<span data-ttu-id="89ecc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89ecc-121">Header</span></span>|<span data-ttu-id="89ecc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89ecc-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="89ecc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ecc-123">Authorization</span></span>  |<span data-ttu-id="89ecc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ecc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89ecc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ecc-126">Request body</span></span>
<span data-ttu-id="89ecc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89ecc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89ecc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ecc-128">Response</span></span>
<span data-ttu-id="89ecc-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ecc-129">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="89ecc-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="89ecc-130">**Request**</span></span>

<span data-ttu-id="89ecc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ecc-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="89ecc-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="89ecc-132">**Response**</span></span>

<span data-ttu-id="89ecc-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ecc-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="89ecc-134">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89ecc-134">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
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
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```



