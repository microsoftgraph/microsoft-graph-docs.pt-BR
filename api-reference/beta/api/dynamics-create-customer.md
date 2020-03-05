---
title: Criar clientes
description: Cria um objeto Customer no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 549c17420790bb0146c4a84b0a5b3a49ca9e3ec9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431729"
---
# <a name="create-customers"></a><span data-ttu-id="45d52-103">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="45d52-103">Create customers</span></span>

<span data-ttu-id="45d52-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45d52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45d52-105">Criar um objeto Customer no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="45d52-105">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="45d52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45d52-106">Permissions</span></span>
<span data-ttu-id="45d52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45d52-109">Permission type</span></span> |<span data-ttu-id="45d52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45d52-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="45d52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45d52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45d52-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d52-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="45d52-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="45d52-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="45d52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45d52-114">Not supported.</span></span>|
|<span data-ttu-id="45d52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45d52-115">Application</span></span>|<span data-ttu-id="45d52-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d52-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45d52-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45d52-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45d52-118">Optional query parameters</span></span>
<span data-ttu-id="45d52-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45d52-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45d52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45d52-120">Request headers</span></span>
|<span data-ttu-id="45d52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45d52-121">Header</span></span>         |<span data-ttu-id="45d52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45d52-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="45d52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45d52-123">Authorization</span></span>  |<span data-ttu-id="45d52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45d52-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="45d52-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45d52-126">Content-Type</span></span>   |<span data-ttu-id="45d52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45d52-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="45d52-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45d52-128">Request body</span></span>
<span data-ttu-id="45d52-129">No corpo da solicitação, forneça uma representação JSON do objeto **Customers** .</span><span class="sxs-lookup"><span data-stu-id="45d52-129">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="45d52-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="45d52-130">Response</span></span>
<span data-ttu-id="45d52-131">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45d52-131">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d52-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45d52-132">Example</span></span>

<span data-ttu-id="45d52-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="45d52-133">**Request**</span></span>

<span data-ttu-id="45d52-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="45d52-134">Here is an example of a request.</span></span>

```json
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

<span data-ttu-id="45d52-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="45d52-135">**Response**</span></span>

<span data-ttu-id="45d52-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45d52-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="45d52-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45d52-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="45d52-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45d52-138">All the properties will be returned from an actual call.</span></span>

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

