---
title: Obter funcionários
description: Obtém um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2309889f58575f2e8b50a6fe3d31c98700d5fb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981319"
---
# <a name="get-employees"></a><span data-ttu-id="a8565-103">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="a8565-103">Get employees</span></span>

<span data-ttu-id="a8565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8565-105">Recupere as propriedades e os relacionamentos de um objeto Employee para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a8565-105">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8565-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8565-106">Permissions</span></span>
<span data-ttu-id="a8565-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8565-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8565-109">Permission type</span></span> |<span data-ttu-id="a8565-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8565-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a8565-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8565-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8565-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8565-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a8565-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8565-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a8565-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8565-114">Not supported.</span></span>|
|<span data-ttu-id="a8565-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8565-115">Application</span></span>|<span data-ttu-id="a8565-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8565-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8565-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8565-117">HTTP request</span></span>
```
GET /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8565-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8565-118">Optional query parameters</span></span>
<span data-ttu-id="a8565-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8565-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8565-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8565-120">Request headers</span></span>
|<span data-ttu-id="a8565-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8565-121">Header</span></span>       |<span data-ttu-id="a8565-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8565-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="a8565-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8565-123">Authorization</span></span>|<span data-ttu-id="a8565-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8565-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8565-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8565-126">Request body</span></span>
<span data-ttu-id="a8565-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8565-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8565-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8565-128">Response</span></span>
<span data-ttu-id="a8565-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **Employees** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8565-129">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="a8565-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a8565-130">**Request**</span></span>

<span data-ttu-id="a8565-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8565-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
```

<span data-ttu-id="a8565-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="a8565-132">**Response**</span></span>

<span data-ttu-id="a8565-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8565-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="a8565-134">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8565-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8565-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8565-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "AH",
  "displayName": "Annette Hill",
  "givenName": "Annette",
  "middleName": "",
  "surname": "Hill",
  "jobTitle": "Secretary",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "email": "",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "terminationDate": "0001-01-01",
  "status": "Active",
  "birthDate": "1973-12-12",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/employees/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"  
}
```




