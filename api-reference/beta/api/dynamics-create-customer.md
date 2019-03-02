---
title: Criar clientes
description: Cria um objeto Customer no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7bf9a6ec0085deb1557a1d65560974d1498e444c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365819"
---
# <a name="create-customers"></a><span data-ttu-id="b0fe7-103">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="b0fe7-103">Create customers</span></span>
<span data-ttu-id="b0fe7-104">Criar um objeto Customer no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-104">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0fe7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0fe7-105">Permissions</span></span>
<span data-ttu-id="b0fe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0fe7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0fe7-108">Permission type</span></span> |<span data-ttu-id="b0fe7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0fe7-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b0fe7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0fe7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b0fe7-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0fe7-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b0fe7-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b0fe7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b0fe7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-113">Not supported.</span></span>|
|<span data-ttu-id="b0fe7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0fe7-114">Application</span></span>|<span data-ttu-id="b0fe7-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0fe7-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0fe7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0fe7-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0fe7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0fe7-117">Optional query parameters</span></span>
<span data-ttu-id="b0fe7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0fe7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fe7-119">Request headers</span></span>
|<span data-ttu-id="b0fe7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0fe7-120">Header</span></span>         |<span data-ttu-id="b0fe7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0fe7-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="b0fe7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0fe7-122">Authorization</span></span>  |<span data-ttu-id="b0fe7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0fe7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0fe7-125">Content-Type</span></span>   |<span data-ttu-id="b0fe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0fe7-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="b0fe7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fe7-127">Request body</span></span>
<span data-ttu-id="b0fe7-128">No corpo da solicitação, forneça uma representação JSON do \*\*\*\* objeto Customers.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-128">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="b0fe7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0fe7-129">Response</span></span>
<span data-ttu-id="b0fe7-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-130">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0fe7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0fe7-131">Example</span></span>

<span data-ttu-id="b0fe7-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b0fe7-132">**Request**</span></span>

<span data-ttu-id="b0fe7-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customers
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

<span data-ttu-id="b0fe7-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="b0fe7-134">**Response**</span></span>

<span data-ttu-id="b0fe7-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="b0fe7-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b0fe7-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0fe7-137">All the properties will be returned from an actual call.</span></span>

```json
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

