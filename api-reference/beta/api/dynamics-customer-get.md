---
title: Obter clientes
description: Obtém um objeto Customer no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0512a493032e738bba41362ecdc40e78de951baf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365840"
---
# <a name="get-customers"></a><span data-ttu-id="a3fb9-103">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="a3fb9-103">Get customers</span></span>
<span data-ttu-id="a3fb9-104">Recupere as propriedades e os relacionamentos de um objeto Customer para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-104">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3fb9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3fb9-105">Permissions</span></span>
<span data-ttu-id="a3fb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3fb9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3fb9-108">Permission type</span></span> |<span data-ttu-id="a3fb9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3fb9-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a3fb9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3fb9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a3fb9-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3fb9-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a3fb9-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a3fb9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a3fb9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-113">Not supported.</span></span>|
|<span data-ttu-id="a3fb9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3fb9-114">Application</span></span>|<span data-ttu-id="a3fb9-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3fb9-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3fb9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3fb9-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3fb9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3fb9-117">Optional query parameters</span></span>
<span data-ttu-id="a3fb9-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3fb9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fb9-119">Request headers</span></span>
|<span data-ttu-id="a3fb9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3fb9-120">Header</span></span>|<span data-ttu-id="a3fb9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a3fb9-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="a3fb9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3fb9-122">Authorization</span></span>  |<span data-ttu-id="a3fb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3fb9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fb9-125">Request body</span></span>
<span data-ttu-id="a3fb9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3fb9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3fb9-127">Response</span></span>
<span data-ttu-id="a3fb9-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-128">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="a3fb9-129">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a3fb9-129">**Request**</span></span>

<span data-ttu-id="a3fb9-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
```

<span data-ttu-id="a3fb9-131">**Response**</span><span class="sxs-lookup"><span data-stu-id="a3fb9-131">**Response**</span></span>

<span data-ttu-id="a3fb9-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="a3fb9-133">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a3fb9-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3fb9-134">All the properties will be returned from an actual call.</span></span>

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

