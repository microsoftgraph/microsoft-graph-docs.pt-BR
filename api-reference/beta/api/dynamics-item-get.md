---
title: Obter itens
description: Obtém um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 622e62e52f97e4fb50efb61537e9831919ca920a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42429780"
---
# <a name="get-items"></a><span data-ttu-id="9ea81-103">Obter itens</span><span class="sxs-lookup"><span data-stu-id="9ea81-103">Get items</span></span>

<span data-ttu-id="9ea81-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9ea81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea81-105">Recupere as propriedades e os relacionamentos de um objeto de item para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="9ea81-105">Retrieve the properties and relationships of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea81-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ea81-106">Permissions</span></span>
<span data-ttu-id="9ea81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ea81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea81-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ea81-109">Permission type</span></span> |<span data-ttu-id="9ea81-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ea81-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9ea81-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ea81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ea81-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea81-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9ea81-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9ea81-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9ea81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ea81-114">Not supported.</span></span>|
|<span data-ttu-id="9ea81-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ea81-115">Application</span></span>|<span data-ttu-id="9ea81-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea81-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ea81-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ea81-117">HTTP request</span></span>

```
GET /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ea81-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ea81-118">Optional query parameters</span></span>
<span data-ttu-id="9ea81-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ea81-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ea81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ea81-120">Request headers</span></span>
|<span data-ttu-id="9ea81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ea81-121">Header</span></span>       |<span data-ttu-id="9ea81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ea81-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="9ea81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ea81-123">Authorization</span></span>|<span data-ttu-id="9ea81-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ea81-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ea81-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ea81-126">Request body</span></span>
<span data-ttu-id="9ea81-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ea81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ea81-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ea81-128">Response</span></span>
<span data-ttu-id="9ea81-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto **Items** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ea81-129">If successful, this method returns a `200 OK` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea81-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ea81-130">Example</span></span>
<span data-ttu-id="9ea81-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="9ea81-131">**Request**</span></span>

<span data-ttu-id="9ea81-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ea81-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="9ea81-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="9ea81-133">**Response**</span></span>

<span data-ttu-id="9ea81-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ea81-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="9ea81-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9ea81-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ea81-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ea81-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "id-value",
  "gtin": "",
  "itemCategoryId": "id-value"
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupId": "id-value",
  "taxGroupCode": "FURNITURE",
  "lastModifiedDateTime": "2017-03-07T00:35:30.073Z"
}

```

