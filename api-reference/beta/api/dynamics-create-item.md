---
title: Criar itens
description: Cria um objeto item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 68bb1e1c8fbfa3c7675b5ef6dc39de24ffad2ecd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365833"
---
# <a name="create-items"></a><span data-ttu-id="bbdb4-103">Criar itens</span><span class="sxs-lookup"><span data-stu-id="bbdb4-103">Create items</span></span>
<span data-ttu-id="bbdb4-104">Criar um item no Dynamics 365 Business central para uso em faturas, citações, etc.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-104">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbdb4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbdb4-105">Permissions</span></span>
<span data-ttu-id="bbdb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbdb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbdb4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbdb4-108">Permission type</span></span> |<span data-ttu-id="bbdb4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbdb4-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bbdb4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbdb4-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bbdb4-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdb4-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bbdb4-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bbdb4-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bbdb4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-113">Not supported.</span></span>|
|<span data-ttu-id="bbdb4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbdb4-114">Application</span></span>|<span data-ttu-id="bbdb4-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdb4-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbdb4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbdb4-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbdb4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bbdb4-117">Optional query parameters</span></span>
<span data-ttu-id="bbdb4-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbdb4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbdb4-119">Request headers</span></span>
|<span data-ttu-id="bbdb4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbdb4-120">Header</span></span>       |<span data-ttu-id="bbdb4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bbdb4-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="bbdb4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbdb4-122">Authorization</span></span>|<span data-ttu-id="bbdb4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bbdb4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbdb4-125">Content-Type</span></span> |<span data-ttu-id="bbdb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbdb4-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="bbdb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbdb4-127">Request body</span></span>
<span data-ttu-id="bbdb4-128">No corpo da solicitação, forneça uma representação JSON de um \*\*\*\* objeto Items.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-128">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="bbdb4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbdb4-129">Response</span></span>
<span data-ttu-id="bbdb4-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto **Items** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-130">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbdb4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbdb4-131">Example</span></span>
<span data-ttu-id="bbdb4-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="bbdb4-132">**Request**</span></span>

<span data-ttu-id="bbdb4-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/items
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

<span data-ttu-id="bbdb4-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="bbdb4-134">**Response**</span></span>

<span data-ttu-id="bbdb4-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="bbdb4-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bbdb4-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbdb4-137">All the properties will be returned from an actual call.</span></span>

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

