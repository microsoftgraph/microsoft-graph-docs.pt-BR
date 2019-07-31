---
title: Criar clientes
description: Cria um objeto Customer no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 5aab0dab11d1b56a9eb230836fe157f87a99a07e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956720"
---
# <a name="create-customers"></a><span data-ttu-id="2d14f-103">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="2d14f-103">Create customers</span></span>
<span data-ttu-id="2d14f-104">Criar um objeto Customer no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2d14f-104">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d14f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d14f-105">Permissions</span></span>
<span data-ttu-id="2d14f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d14f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d14f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d14f-108">Permission type</span></span> |<span data-ttu-id="2d14f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d14f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2d14f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d14f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2d14f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d14f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2d14f-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2d14f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2d14f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d14f-113">Not supported.</span></span>|
|<span data-ttu-id="2d14f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d14f-114">Application</span></span>|<span data-ttu-id="2d14f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d14f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d14f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d14f-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d14f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2d14f-117">Optional query parameters</span></span>
<span data-ttu-id="2d14f-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2d14f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d14f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d14f-119">Request headers</span></span>
|<span data-ttu-id="2d14f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d14f-120">Header</span></span>         |<span data-ttu-id="2d14f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d14f-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="2d14f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d14f-122">Authorization</span></span>  |<span data-ttu-id="2d14f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d14f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d14f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d14f-125">Content-Type</span></span>   |<span data-ttu-id="2d14f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d14f-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="2d14f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d14f-127">Request body</span></span>
<span data-ttu-id="2d14f-128">No corpo da solicitação, forneça uma representação JSON do \*\*\*\* objeto Customers.</span><span class="sxs-lookup"><span data-stu-id="2d14f-128">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="2d14f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d14f-129">Response</span></span>
<span data-ttu-id="2d14f-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Customers** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d14f-130">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d14f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d14f-131">Example</span></span>

<span data-ttu-id="2d14f-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="2d14f-132">**Request**</span></span>

<span data-ttu-id="2d14f-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d14f-133">Here is an example of a request.</span></span>

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

<span data-ttu-id="2d14f-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="2d14f-134">**Response**</span></span>

<span data-ttu-id="2d14f-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d14f-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="2d14f-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2d14f-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2d14f-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d14f-137">All the properties will be returned from an actual call.</span></span>

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

