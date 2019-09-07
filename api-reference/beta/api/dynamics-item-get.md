---
title: Obter itens
description: Obtém um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 13977c32081e438f6b31e80bd76084ec1a4725c0
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791565"
---
# <a name="get-items"></a><span data-ttu-id="87404-103">Obter itens</span><span class="sxs-lookup"><span data-stu-id="87404-103">Get items</span></span>
<span data-ttu-id="87404-104">Recupere as propriedades e os relacionamentos de um objeto de item para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="87404-104">Retrieve the properties and relationships of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="87404-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="87404-105">Permissions</span></span>
<span data-ttu-id="87404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87404-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87404-108">Permission type</span></span> |<span data-ttu-id="87404-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87404-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="87404-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87404-110">Delegated (work or school account)</span></span>|<span data-ttu-id="87404-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87404-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="87404-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="87404-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="87404-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87404-113">Not supported.</span></span>|
|<span data-ttu-id="87404-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87404-114">Application</span></span>|<span data-ttu-id="87404-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87404-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87404-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87404-116">HTTP request</span></span>

```
GET /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87404-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87404-117">Optional query parameters</span></span>
<span data-ttu-id="87404-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87404-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87404-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87404-119">Request headers</span></span>
|<span data-ttu-id="87404-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87404-120">Header</span></span>       |<span data-ttu-id="87404-121">Valor</span><span class="sxs-lookup"><span data-stu-id="87404-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="87404-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87404-122">Authorization</span></span>|<span data-ttu-id="87404-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87404-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87404-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87404-125">Request body</span></span>
<span data-ttu-id="87404-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87404-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87404-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="87404-127">Response</span></span>
<span data-ttu-id="87404-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto **Items** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87404-128">If successful, this method returns a `200 OK` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87404-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87404-129">Example</span></span>
<span data-ttu-id="87404-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="87404-130">**Request**</span></span>

<span data-ttu-id="87404-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87404-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="87404-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="87404-132">**Response**</span></span>

<span data-ttu-id="87404-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87404-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="87404-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="87404-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="87404-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87404-135">All the properties will be returned from an actual call.</span></span>

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

