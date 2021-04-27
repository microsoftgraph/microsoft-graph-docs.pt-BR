---
title: Criar clientes
description: Cria um objeto do cliente no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b7fc4cedfd4476860e04ee24333b064741d5d85f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045975"
---
# <a name="create-customers"></a><span data-ttu-id="734c0-103">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="734c0-103">Create customers</span></span>

<span data-ttu-id="734c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="734c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="734c0-105">Crie um objeto do cliente no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="734c0-105">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="734c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="734c0-106">Permissions</span></span>
<span data-ttu-id="734c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="734c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="734c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="734c0-109">Permission type</span></span> |<span data-ttu-id="734c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="734c0-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="734c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="734c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="734c0-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734c0-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="734c0-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="734c0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="734c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="734c0-114">Not supported.</span></span>|
|<span data-ttu-id="734c0-115">Application</span><span class="sxs-lookup"><span data-stu-id="734c0-115">Application</span></span>|<span data-ttu-id="734c0-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="734c0-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="734c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="734c0-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="734c0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="734c0-118">Optional query parameters</span></span>
<span data-ttu-id="734c0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="734c0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="734c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="734c0-120">Request headers</span></span>
|<span data-ttu-id="734c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="734c0-121">Header</span></span>         |<span data-ttu-id="734c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="734c0-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="734c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="734c0-123">Authorization</span></span>  |<span data-ttu-id="734c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="734c0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="734c0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="734c0-126">Content-Type</span></span>   |<span data-ttu-id="734c0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="734c0-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="734c0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="734c0-128">Request body</span></span>
<span data-ttu-id="734c0-129">No corpo da solicitação, fornece uma representação JSON do **objeto customers.**</span><span class="sxs-lookup"><span data-stu-id="734c0-129">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="734c0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="734c0-130">Response</span></span>
<span data-ttu-id="734c0-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="734c0-131">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="734c0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="734c0-132">Example</span></span>

<span data-ttu-id="734c0-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="734c0-133">**Request**</span></span>

<span data-ttu-id="734c0-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="734c0-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/customers
Content-type: application/json

{
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
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
}

```

<span data-ttu-id="734c0-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="734c0-135">**Response**</span></span>

<span data-ttu-id="734c0-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="734c0-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="734c0-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="734c0-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "currencyCode": "USD",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}

```



