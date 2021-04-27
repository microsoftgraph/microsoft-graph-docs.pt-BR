---
title: Atualizar funcionários
description: Atualiza um objeto de funcionário no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8940e5ff851ea2b61aa286ee8637cd8ab847821c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045387"
---
# <a name="update-employees"></a><span data-ttu-id="b3a80-103">Atualizar funcionários</span><span class="sxs-lookup"><span data-stu-id="b3a80-103">Update employees</span></span>

<span data-ttu-id="b3a80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3a80-105">Atualize as propriedades de um objeto de funcionário para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b3a80-105">Update the properties of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3a80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3a80-106">Permissions</span></span>
<span data-ttu-id="b3a80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3a80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3a80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3a80-109">Permission type</span></span> |<span data-ttu-id="b3a80-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3a80-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b3a80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3a80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3a80-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a80-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b3a80-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b3a80-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b3a80-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3a80-114">Not supported.</span></span>|
|<span data-ttu-id="b3a80-115">Application</span><span class="sxs-lookup"><span data-stu-id="b3a80-115">Application</span></span>|<span data-ttu-id="b3a80-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a80-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3a80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3a80-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/employees/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3a80-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3a80-118">Optional query parameters</span></span>
<span data-ttu-id="b3a80-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3a80-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3a80-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3a80-120">Request headers</span></span>
|<span data-ttu-id="b3a80-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3a80-121">Header</span></span>         |<span data-ttu-id="b3a80-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3a80-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="b3a80-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3a80-123">Authorization</span></span>  |<span data-ttu-id="b3a80-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3a80-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b3a80-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3a80-126">Content-Type</span></span>   |<span data-ttu-id="b3a80-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="b3a80-127">application/json.</span></span>         |
|<span data-ttu-id="b3a80-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="b3a80-128">If-Match</span></span>       |<span data-ttu-id="b3a80-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3a80-129">Required.</span></span> <span data-ttu-id="b3a80-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual dos funcionários, os funcionários **não** serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="b3a80-130">When this request header is included and the eTag provided does not match the current tag on the **employees**, the **employees** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3a80-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3a80-131">Request body</span></span>
<span data-ttu-id="b3a80-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b3a80-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b3a80-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3a80-135">Response</span></span>
<span data-ttu-id="b3a80-136">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto de **funcionários** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3a80-136">If successful, this method returns a `200 OK` response code and an updated **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3a80-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3a80-137">Example</span></span>

<span data-ttu-id="b3a80-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b3a80-138">**Request**</span></span>

<span data-ttu-id="b3a80-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3a80-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/employees/{id}
Content-type: application/json

{
  "givenName": "Anthony",
  "phoneNumber": "0678-8712-3455"
}
```

<span data-ttu-id="b3a80-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="b3a80-140">**Response**</span></span>

<span data-ttu-id="b3a80-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3a80-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="b3a80-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b3a80-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "displayName": "Anthony Hill",
  "givenName": "Anthony",
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
  "phoneNumber": "0678-8712-3455",
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
  


