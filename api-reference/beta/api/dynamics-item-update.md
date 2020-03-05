---
title: Atualizar itens
description: Atualiza um objeto item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 351104ff934c5390dfb30a57b3a93d0623cb7d9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42429584"
---
# <a name="update-items"></a><span data-ttu-id="3a8a3-103">Atualizar itens</span><span class="sxs-lookup"><span data-stu-id="3a8a3-103">Update items</span></span>

<span data-ttu-id="3a8a3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3a8a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a8a3-105">Atualizar as propriedades de um objeto de item para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-105">Update the properties of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a8a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a8a3-106">Permissions</span></span>
<span data-ttu-id="3a8a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a8a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a8a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a8a3-109">Permission type</span></span> |<span data-ttu-id="3a8a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a8a3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3a8a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a8a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a8a3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a8a3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3a8a3-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3a8a3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3a8a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-114">Not supported.</span></span>|
|<span data-ttu-id="3a8a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a8a3-115">Application</span></span>|<span data-ttu-id="3a8a3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a8a3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a8a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a8a3-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a8a3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a8a3-118">Optional query parameters</span></span>
<span data-ttu-id="3a8a3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a8a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a8a3-120">Request headers</span></span>
|<span data-ttu-id="3a8a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a8a3-121">Header</span></span>       |<span data-ttu-id="3a8a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a8a3-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="3a8a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a8a3-123">Authorization</span></span>|<span data-ttu-id="3a8a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3a8a3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a8a3-126">Content-Type</span></span> |<span data-ttu-id="3a8a3-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-127">application/json.</span></span>        |
|<span data-ttu-id="3a8a3-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="3a8a3-128">If-Match</span></span>     |<span data-ttu-id="3a8a3-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-129">Required.</span></span> <span data-ttu-id="3a8a3-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos **itens**, os **itens** não serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-130">When this request header is included and the eTag provided does not match the current tag on the **items**, the **items** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a8a3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a8a3-131">Request body</span></span>
<span data-ttu-id="3a8a3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="3a8a3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a8a3-135">Response</span></span>
<span data-ttu-id="3a8a3-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Items** atualizados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-136">If successful, this method returns a `200 OK` response code and an updated **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a8a3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a8a3-137">Example</span></span>
<span data-ttu-id="3a8a3-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="3a8a3-138">**Request**</span></span>

<span data-ttu-id="3a8a3-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
Content-type: application/json

{
  "displayName": "ATHENS Desk - blocked",
  "blocked": true
}
```

<span data-ttu-id="3a8a3-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="3a8a3-140">**Response**</span></span>

<span data-ttu-id="3a8a3-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="3a8a3-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a8a3-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a8a3-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk - blocked",
  "type": "Inventory",
  "blocked": true,
  "baseUnitOfMeasureId": "id-value", 
  "gtin": "",
  "itemCategoryId": "id-value",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupId": "id-value",
  "taxGroupCode": "FURNITURE",
  "lastModifiedDateTime": "2017-03-07T00:35:30.073Z"
}

```


