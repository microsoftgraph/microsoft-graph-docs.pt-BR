---
title: Obter funcionários
description: Obtém um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9adab4c18d2c380f949d3fd7894aae4a8de7c0da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458450"
---
# <a name="get-employees"></a><span data-ttu-id="5d5f5-103">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="5d5f5-103">Get employees</span></span>
<span data-ttu-id="5d5f5-104">Recupere as propriedades e os relacionamentos de um objeto Employee para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-104">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d5f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d5f5-105">Permissions</span></span>
<span data-ttu-id="5d5f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d5f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d5f5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d5f5-108">Permission type</span></span> |<span data-ttu-id="5d5f5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d5f5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5d5f5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d5f5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5d5f5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5f5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5d5f5-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d5f5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5d5f5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-113">Not supported.</span></span>|
|<span data-ttu-id="5d5f5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d5f5-114">Application</span></span>|<span data-ttu-id="5d5f5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5f5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d5f5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d5f5-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/employees('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d5f5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d5f5-117">Optional query parameters</span></span>
<span data-ttu-id="5d5f5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d5f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d5f5-119">Request headers</span></span>
|<span data-ttu-id="5d5f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d5f5-120">Header</span></span>       |<span data-ttu-id="5d5f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5d5f5-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="5d5f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d5f5-122">Authorization</span></span>|<span data-ttu-id="5d5f5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d5f5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d5f5-125">Request body</span></span>
<span data-ttu-id="5d5f5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d5f5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d5f5-127">Response</span></span>
<span data-ttu-id="5d5f5-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Employees** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-128">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="5d5f5-129">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="5d5f5-129">**Request**</span></span>

<span data-ttu-id="5d5f5-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/employees('{id}')
```

<span data-ttu-id="5d5f5-131">**Response**</span><span class="sxs-lookup"><span data-stu-id="5d5f5-131">**Response**</span></span>

<span data-ttu-id="5d5f5-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="5d5f5-133">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d5f5-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d5f5-134">All the properties will be returned from an actual call.</span></span>

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
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/employees('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"  
}
```


