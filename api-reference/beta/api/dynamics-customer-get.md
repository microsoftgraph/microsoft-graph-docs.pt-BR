---
title: Obter clientes
description: Obtém um objeto Customer no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ffc6ab031045aeadcdb44166e6bc17cf5e01f5f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981482"
---
# <a name="get-customers"></a><span data-ttu-id="34e29-103">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="34e29-103">Get customers</span></span>

<span data-ttu-id="34e29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34e29-105">Recupere as propriedades e os relacionamentos de um objeto Customer para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="34e29-105">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="34e29-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34e29-106">Permissions</span></span>
<span data-ttu-id="34e29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34e29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34e29-109">Permission type</span></span> |<span data-ttu-id="34e29-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34e29-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="34e29-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34e29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34e29-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e29-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="34e29-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="34e29-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="34e29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34e29-114">Not supported.</span></span>|
|<span data-ttu-id="34e29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34e29-115">Application</span></span>|<span data-ttu-id="34e29-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e29-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34e29-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34e29-117">HTTP request</span></span>
```
GET /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34e29-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34e29-118">Optional query parameters</span></span>
<span data-ttu-id="34e29-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34e29-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e29-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34e29-120">Request headers</span></span>
|<span data-ttu-id="34e29-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34e29-121">Header</span></span>|<span data-ttu-id="34e29-122">Valor</span><span class="sxs-lookup"><span data-stu-id="34e29-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="34e29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34e29-123">Authorization</span></span>  |<span data-ttu-id="34e29-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34e29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34e29-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34e29-126">Request body</span></span>
<span data-ttu-id="34e29-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34e29-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34e29-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="34e29-128">Response</span></span>
<span data-ttu-id="34e29-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **Customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34e29-129">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="34e29-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="34e29-130">**Request**</span></span>

<span data-ttu-id="34e29-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34e29-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="34e29-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="34e29-132">**Response**</span></span>

<span data-ttu-id="34e29-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34e29-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="34e29-134">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34e29-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="34e29-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34e29-135">All the properties will be returned from an actual call.</span></span>

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



