---
title: Obter moedas
description: Obtém um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6c8d3fdf8c6251e4764cfd61a484c287af58e53f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430942"
---
# <a name="get-currencies"></a><span data-ttu-id="a73d3-103">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="a73d3-103">Get currencies</span></span>

<span data-ttu-id="a73d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a73d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a73d3-105">Recupere as propriedades e os relacionamentos de um objeto Currency para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a73d3-105">Retrieve the properties and relationships of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a73d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a73d3-106">Permissions</span></span>
<span data-ttu-id="a73d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a73d3-109">Permission type</span></span> |<span data-ttu-id="a73d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a73d3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a73d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a73d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a73d3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73d3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a73d3-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a73d3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a73d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a73d3-114">Not supported.</span></span>|
|<span data-ttu-id="a73d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a73d3-115">Application</span></span>|<span data-ttu-id="a73d3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73d3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a73d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a73d3-117">HTTP request</span></span>

```
GET /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a73d3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a73d3-118">Optional query parameters</span></span>
<span data-ttu-id="a73d3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a73d3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a73d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a73d3-120">Request headers</span></span>
|<span data-ttu-id="a73d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a73d3-121">Header</span></span>|<span data-ttu-id="a73d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a73d3-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a73d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a73d3-123">Authorization</span></span>  |<span data-ttu-id="a73d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a73d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a73d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a73d3-126">Request body</span></span>
<span data-ttu-id="a73d3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a73d3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a73d3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a73d3-128">Response</span></span>
<span data-ttu-id="a73d3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **moedas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a73d3-129">If successful, this method returns a `200 OK` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a73d3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a73d3-130">Example</span></span>

<span data-ttu-id="a73d3-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a73d3-131">**Request**</span></span>

<span data-ttu-id="a73d3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a73d3-132">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="a73d3-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="a73d3-133">**Response**</span></span>

<span data-ttu-id="a73d3-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a73d3-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="a73d3-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a73d3-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a73d3-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a73d3-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.003Z"
}
```
