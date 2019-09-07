---
title: Criar fornecedores
description: Cria um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4595fca85d85bab0eaec1629a4422c1db5fa9964
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791852"
---
# <a name="create-vendors"></a><span data-ttu-id="b4b81-103">Criar fornecedores</span><span class="sxs-lookup"><span data-stu-id="b4b81-103">Create vendors</span></span>
<span data-ttu-id="b4b81-104">Criar um objeto fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b4b81-104">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4b81-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4b81-105">Permissions</span></span>
<span data-ttu-id="b4b81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b81-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4b81-108">Permission type</span></span> |<span data-ttu-id="b4b81-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4b81-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b4b81-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4b81-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b81-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b81-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b4b81-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b4b81-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b4b81-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4b81-113">Not supported.</span></span>|
|<span data-ttu-id="b4b81-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4b81-114">Application</span></span>|<span data-ttu-id="b4b81-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b81-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b81-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4b81-116">HTTP request</span></span>
```
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4b81-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4b81-117">Optional query parameters</span></span>
<span data-ttu-id="b4b81-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4b81-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4b81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4b81-119">Request headers</span></span>
|<span data-ttu-id="b4b81-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4b81-120">Header</span></span>|<span data-ttu-id="b4b81-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4b81-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="b4b81-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4b81-122">Authorization</span></span>  |<span data-ttu-id="b4b81-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4b81-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b4b81-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4b81-125">Content-Type</span></span>  |<span data-ttu-id="b4b81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b81-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="b4b81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4b81-127">Request body</span></span>
<span data-ttu-id="b4b81-128">No corpo da solicitação, forneça uma representação JSON de um objeto **fornecedores** .</span><span class="sxs-lookup"><span data-stu-id="b4b81-128">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="b4b81-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4b81-129">Response</span></span>
<span data-ttu-id="b4b81-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **fornecedores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4b81-130">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b81-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4b81-131">Example</span></span>

<span data-ttu-id="b4b81-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b4b81-132">**Request**</span></span>

<span data-ttu-id="b4b81-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4b81-133">Here is an example of a request.</span></span>

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

<span data-ttu-id="b4b81-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="b4b81-134">**Response**</span></span>

<span data-ttu-id="b4b81-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4b81-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="b4b81-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b4b81-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4b81-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4b81-137">All the properties will be returned from an actual call.</span></span>

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

