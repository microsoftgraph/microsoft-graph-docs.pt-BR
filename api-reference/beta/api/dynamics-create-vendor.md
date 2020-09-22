---
title: Criar fornecedores
description: Cria um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b0a85dd1d177f5a6ac3caea8054e6bc0aa5aeb0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981545"
---
# <a name="create-vendors"></a><span data-ttu-id="40421-103">Criar fornecedores</span><span class="sxs-lookup"><span data-stu-id="40421-103">Create vendors</span></span>

<span data-ttu-id="40421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40421-105">Criar um objeto fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="40421-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="40421-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="40421-106">Permissions</span></span>
<span data-ttu-id="40421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40421-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40421-109">Permission type</span></span> |<span data-ttu-id="40421-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40421-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="40421-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40421-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40421-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40421-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="40421-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="40421-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="40421-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40421-114">Not supported.</span></span>|
|<span data-ttu-id="40421-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40421-115">Application</span></span>|<span data-ttu-id="40421-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40421-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40421-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40421-117">HTTP request</span></span>
```
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40421-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40421-118">Optional query parameters</span></span>
<span data-ttu-id="40421-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40421-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40421-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40421-120">Request headers</span></span>
|<span data-ttu-id="40421-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40421-121">Header</span></span>|<span data-ttu-id="40421-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40421-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="40421-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40421-123">Authorization</span></span>  |<span data-ttu-id="40421-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40421-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="40421-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40421-126">Content-Type</span></span>  |<span data-ttu-id="40421-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40421-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="40421-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40421-128">Request body</span></span>
<span data-ttu-id="40421-129">No corpo da solicitação, forneça uma representação JSON de um objeto **fornecedores** .</span><span class="sxs-lookup"><span data-stu-id="40421-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="40421-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="40421-130">Response</span></span>
<span data-ttu-id="40421-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **fornecedores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40421-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40421-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40421-132">Example</span></span>

<span data-ttu-id="40421-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="40421-133">**Request**</span></span>

<span data-ttu-id="40421-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="40421-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/vendors
Content-type: application/json

{
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="40421-135">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="40421-135">**Response**</span></span>

<span data-ttu-id="40421-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40421-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="40421-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40421-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40421-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40421-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}

```



