---
title: Criar funcionários
description: Cria um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: bb1bc0754d921f6c979f78cec5a496c5ad52bd9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981699"
---
# <a name="create-employees"></a><span data-ttu-id="3aae0-103">Criar funcionários</span><span class="sxs-lookup"><span data-stu-id="3aae0-103">Create employees</span></span>

<span data-ttu-id="3aae0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aae0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aae0-105">Criar um objeto Employee no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3aae0-105">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aae0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aae0-106">Permissions</span></span>
<span data-ttu-id="3aae0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aae0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aae0-109">Permission type</span></span> |<span data-ttu-id="3aae0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aae0-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3aae0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aae0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3aae0-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aae0-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3aae0-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3aae0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3aae0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aae0-114">Not supported.</span></span>|
|<span data-ttu-id="3aae0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aae0-115">Application</span></span>|<span data-ttu-id="3aae0-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aae0-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aae0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aae0-117">HTTP request</span></span>
```
POST /financials/companies/{id}/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3aae0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3aae0-118">Optional query parameters</span></span>
<span data-ttu-id="3aae0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3aae0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aae0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aae0-120">Request headers</span></span>
|<span data-ttu-id="3aae0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3aae0-121">Header</span></span>        |<span data-ttu-id="3aae0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3aae0-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="3aae0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aae0-123">Authorization</span></span> |<span data-ttu-id="3aae0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aae0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3aae0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3aae0-126">Content-Type</span></span>  |<span data-ttu-id="3aae0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3aae0-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="3aae0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aae0-128">Request body</span></span>
<span data-ttu-id="3aae0-129">No corpo da solicitação, forneça uma representação JSON de um objeto **Employees** .</span><span class="sxs-lookup"><span data-stu-id="3aae0-129">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="3aae0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aae0-130">Response</span></span>
<span data-ttu-id="3aae0-131">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Employees** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aae0-131">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aae0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aae0-132">Example</span></span>

<span data-ttu-id="3aae0-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="3aae0-133">**Request**</span></span>

<span data-ttu-id="3aae0-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aae0-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/employees
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "givenName": "Annette",
  "surname": "Hill",
  "jobTitle": "Production Assistant",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "birthDate": "1973-12-12"  
}

```

<span data-ttu-id="3aae0-135">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="3aae0-135">**Response**</span></span>

<span data-ttu-id="3aae0-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aae0-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="3aae0-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3aae0-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3aae0-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aae0-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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



