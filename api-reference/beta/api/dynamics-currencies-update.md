---
title: Atualizar moedas
description: Atualiza um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ccbd21cfa327865e2c7fc10aa98355bd3a68cde8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430900"
---
# <a name="update-currencies"></a><span data-ttu-id="eb2fa-103">Atualizar moedas</span><span class="sxs-lookup"><span data-stu-id="eb2fa-103">Update currencies</span></span>

<span data-ttu-id="eb2fa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb2fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb2fa-105">Atualizar as propriedades de um objeto Currency para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-105">Update the properties of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb2fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb2fa-106">Permissions</span></span>
<span data-ttu-id="eb2fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb2fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb2fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb2fa-109">Permission type</span></span> |<span data-ttu-id="eb2fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb2fa-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="eb2fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb2fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb2fa-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb2fa-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="eb2fa-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="eb2fa-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eb2fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-114">Not supported.</span></span>|
|<span data-ttu-id="eb2fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb2fa-115">Application</span></span>|<span data-ttu-id="eb2fa-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb2fa-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb2fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb2fa-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb2fa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb2fa-118">Optional query parameters</span></span>
<span data-ttu-id="eb2fa-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb2fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2fa-120">Request headers</span></span>
|<span data-ttu-id="eb2fa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb2fa-121">Header</span></span>       |<span data-ttu-id="eb2fa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb2fa-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="eb2fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb2fa-123">Authorization</span></span>|<span data-ttu-id="eb2fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eb2fa-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb2fa-126">Content-Type</span></span> |<span data-ttu-id="eb2fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb2fa-127">application/json</span></span>         |
|<span data-ttu-id="eb2fa-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="eb2fa-128">If-Match</span></span>     |<span data-ttu-id="eb2fa-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-129">Required.</span></span> <span data-ttu-id="eb2fa-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **moedas**, as **moedas** não serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-130">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb2fa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2fa-131">Request body</span></span>
<span data-ttu-id="eb2fa-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="eb2fa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb2fa-135">Response</span></span>
<span data-ttu-id="eb2fa-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de **moedas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-136">If successful, this method returns a `200 OK` response code and an updated **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2fa-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb2fa-137">Example</span></span>

<span data-ttu-id="eb2fa-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="eb2fa-138">**Request**</span></span>

<span data-ttu-id="eb2fa-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

<span data-ttu-id="eb2fa-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="eb2fa-140">**Response**</span></span>

<span data-ttu-id="eb2fa-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="eb2fa-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb2fa-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb2fa-143">All the properties will be returned from an actual call.</span></span>

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
