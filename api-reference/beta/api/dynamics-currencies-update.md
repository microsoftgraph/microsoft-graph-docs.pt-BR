---
title: Atualizar moedas
description: Atualiza um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 47a0b61c56a83199101d9fba1758464e8b35d99c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791810"
---
# <a name="update-currencies"></a><span data-ttu-id="d92f6-103">Atualizar moedas</span><span class="sxs-lookup"><span data-stu-id="d92f6-103">Update currencies</span></span>
<span data-ttu-id="d92f6-104">Atualizar as propriedades de um objeto Currency para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="d92f6-104">Update the properties of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d92f6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d92f6-105">Permissions</span></span>
<span data-ttu-id="d92f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d92f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d92f6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d92f6-108">Permission type</span></span> |<span data-ttu-id="d92f6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d92f6-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d92f6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d92f6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d92f6-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92f6-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d92f6-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d92f6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d92f6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d92f6-113">Not supported.</span></span>|
|<span data-ttu-id="d92f6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d92f6-114">Application</span></span>|<span data-ttu-id="d92f6-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92f6-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d92f6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d92f6-116">HTTP request</span></span>
```
PATCH /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d92f6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d92f6-117">Optional query parameters</span></span>
<span data-ttu-id="d92f6-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d92f6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d92f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d92f6-119">Request headers</span></span>
|<span data-ttu-id="d92f6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d92f6-120">Header</span></span>       |<span data-ttu-id="d92f6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d92f6-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="d92f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d92f6-122">Authorization</span></span>|<span data-ttu-id="d92f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d92f6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d92f6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d92f6-125">Content-Type</span></span> |<span data-ttu-id="d92f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d92f6-126">application/json</span></span>         |
|<span data-ttu-id="d92f6-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="d92f6-127">If-Match</span></span>     |<span data-ttu-id="d92f6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d92f6-128">Required.</span></span> <span data-ttu-id="d92f6-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **moedas**, as **moedas** não serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d92f6-129">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d92f6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d92f6-130">Request body</span></span>
<span data-ttu-id="d92f6-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d92f6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d92f6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d92f6-134">Response</span></span>
<span data-ttu-id="d92f6-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de **moedas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d92f6-135">If successful, this method returns a `200 OK` response code and an updated **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d92f6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d92f6-136">Example</span></span>

<span data-ttu-id="d92f6-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="d92f6-137">**Request**</span></span>

<span data-ttu-id="d92f6-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d92f6-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

<span data-ttu-id="d92f6-139">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="d92f6-139">**Response**</span></span>

<span data-ttu-id="d92f6-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d92f6-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="d92f6-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d92f6-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d92f6-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d92f6-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:12:18.793Z"
}
```
