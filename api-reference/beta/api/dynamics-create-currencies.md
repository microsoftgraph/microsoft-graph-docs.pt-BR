---
title: Criar moedas
description: Cria um objeto currency no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 941a22ebccbe0d55bba3f64bab237d0478327529
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046003"
---
# <a name="create-currencies"></a><span data-ttu-id="3dfd4-103">Criar moedas</span><span class="sxs-lookup"><span data-stu-id="3dfd4-103">Create currencies</span></span>

<span data-ttu-id="3dfd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dfd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfd4-105">Crie um objeto currency no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-105">Create a currency object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dfd4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dfd4-106">Permissions</span></span>
<span data-ttu-id="3dfd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dfd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dfd4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dfd4-109">Permission type</span></span> |<span data-ttu-id="3dfd4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dfd4-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3dfd4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dfd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3dfd4-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfd4-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3dfd4-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3dfd4-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3dfd4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-114">Not supported.</span></span>|
|<span data-ttu-id="3dfd4-115">Application</span><span class="sxs-lookup"><span data-stu-id="3dfd4-115">Application</span></span>|<span data-ttu-id="3dfd4-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfd4-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dfd4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfd4-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/currencies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dfd4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3dfd4-118">Optional query parameters</span></span>
<span data-ttu-id="3dfd4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dfd4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfd4-120">Request headers</span></span>
|<span data-ttu-id="3dfd4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3dfd4-121">Header</span></span>         |<span data-ttu-id="3dfd4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3dfd4-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="3dfd4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dfd4-123">Authorization</span></span>  |<span data-ttu-id="3dfd4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3dfd4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3dfd4-126">Content-Type</span></span>   |<span data-ttu-id="3dfd4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3dfd4-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="3dfd4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dfd4-128">Request body</span></span>
<span data-ttu-id="3dfd4-129">No corpo da solicitação, fornece uma representação JSON do **objeto currencies.**</span><span class="sxs-lookup"><span data-stu-id="3dfd4-129">In the request body, supply a JSON representation of **currencies** object.</span></span>

## <a name="response"></a><span data-ttu-id="3dfd4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dfd4-130">Response</span></span>
<span data-ttu-id="3dfd4-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto de **moedas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-131">If successful, this method returns ```201 Created``` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfd4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dfd4-132">Example</span></span>

<span data-ttu-id="3dfd4-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="3dfd4-133">**Request**</span></span>

<span data-ttu-id="3dfd4-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/currencies
Content-type: application/json

{
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01
}
```

<span data-ttu-id="3dfd4-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="3dfd4-135">**Response**</span></span>

<span data-ttu-id="3dfd4-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="3dfd4-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3dfd4-137">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.002Z"
}

```


