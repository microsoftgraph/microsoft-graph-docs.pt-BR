---
title: Criar funcionários
description: Cria um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7be8690da317a727cc93cbe95ba0a7b52ab7aab0
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791999"
---
# <a name="create-employees"></a><span data-ttu-id="826bb-103">Criar funcionários</span><span class="sxs-lookup"><span data-stu-id="826bb-103">Create employees</span></span>
<span data-ttu-id="826bb-104">Criar um objeto Employee no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="826bb-104">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="826bb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="826bb-105">Permissions</span></span>
<span data-ttu-id="826bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="826bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="826bb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="826bb-108">Permission type</span></span> |<span data-ttu-id="826bb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="826bb-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="826bb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="826bb-110">Delegated (work or school account)</span></span>|<span data-ttu-id="826bb-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="826bb-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="826bb-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="826bb-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="826bb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="826bb-113">Not supported.</span></span>|
|<span data-ttu-id="826bb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="826bb-114">Application</span></span>|<span data-ttu-id="826bb-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="826bb-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="826bb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="826bb-116">HTTP request</span></span>
```
POST /financials/companies/{id}/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="826bb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="826bb-117">Optional query parameters</span></span>
<span data-ttu-id="826bb-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="826bb-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="826bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="826bb-119">Request headers</span></span>
|<span data-ttu-id="826bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="826bb-120">Header</span></span>        |<span data-ttu-id="826bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="826bb-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="826bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="826bb-122">Authorization</span></span> |<span data-ttu-id="826bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="826bb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="826bb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="826bb-125">Content-Type</span></span>  |<span data-ttu-id="826bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="826bb-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="826bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="826bb-127">Request body</span></span>
<span data-ttu-id="826bb-128">No corpo da solicitação, forneça uma representação JSON de um objeto **Employees** .</span><span class="sxs-lookup"><span data-stu-id="826bb-128">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="826bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="826bb-129">Response</span></span>
<span data-ttu-id="826bb-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Employees** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="826bb-130">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="826bb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="826bb-131">Example</span></span>

<span data-ttu-id="826bb-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="826bb-132">**Request**</span></span>

<span data-ttu-id="826bb-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="826bb-133">Here is an example of a request.</span></span>

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

<span data-ttu-id="826bb-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="826bb-134">**Response**</span></span>

<span data-ttu-id="826bb-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="826bb-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="826bb-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="826bb-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="826bb-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="826bb-137">All the properties will be returned from an actual call.</span></span>

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

