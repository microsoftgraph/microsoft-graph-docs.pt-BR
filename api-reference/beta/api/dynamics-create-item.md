---
title: Criar itens
description: Cria um objeto item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: eeeb6a2143963803dc9b6ba06a2e780d7c7fab02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431512"
---
# <a name="create-items"></a><span data-ttu-id="ee4ea-103">Criar itens</span><span class="sxs-lookup"><span data-stu-id="ee4ea-103">Create items</span></span>

<span data-ttu-id="ee4ea-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee4ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee4ea-105">Criar um item no Dynamics 365 Business central para uso em faturas, citações, etc.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-105">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee4ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee4ea-106">Permissions</span></span>
<span data-ttu-id="ee4ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee4ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee4ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee4ea-109">Permission type</span></span> |<span data-ttu-id="ee4ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee4ea-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ee4ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee4ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee4ea-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4ea-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ee4ea-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ee4ea-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ee4ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-114">Not supported.</span></span>|
|<span data-ttu-id="ee4ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee4ea-115">Application</span></span>|<span data-ttu-id="ee4ea-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4ea-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee4ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee4ea-117">HTTP request</span></span>
```
POST /financials/companies/{id}/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee4ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee4ea-118">Optional query parameters</span></span>
<span data-ttu-id="ee4ea-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee4ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4ea-120">Request headers</span></span>
|<span data-ttu-id="ee4ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee4ea-121">Header</span></span>       |<span data-ttu-id="ee4ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee4ea-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="ee4ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee4ea-123">Authorization</span></span>|<span data-ttu-id="ee4ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee4ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee4ea-126">Content-Type</span></span> |<span data-ttu-id="ee4ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee4ea-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="ee4ea-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4ea-128">Request body</span></span>
<span data-ttu-id="ee4ea-129">No corpo da solicitação, forneça uma representação JSON de um objeto **Items** .</span><span class="sxs-lookup"><span data-stu-id="ee4ea-129">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="ee4ea-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee4ea-130">Response</span></span>
<span data-ttu-id="ee4ea-131">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Items** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-131">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee4ea-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee4ea-132">Example</span></span>
<span data-ttu-id="ee4ea-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="ee4ea-133">**Request**</span></span>

<span data-ttu-id="ee4ea-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/items
Content-type: application/json

{
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "65bdbd3a-39f1-49f4-bf24-598cbac36230",
  "gtin": "",
  "itemCategoryId": "5b0b9c1c-312d-4809-96b2-056690a11057",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupCode": "FURNITURE"
} 

```

<span data-ttu-id="ee4ea-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="ee4ea-135">**Response**</span></span>

<span data-ttu-id="ee4ea-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="ee4ea-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ee4ea-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee4ea-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```

