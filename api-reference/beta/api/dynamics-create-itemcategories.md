---
title: Criar categorias de categoria
description: Cria um objeto de categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3ecf5df6dbd03014ba026ba8673c9a4b2fffd5b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431477"
---
# <a name="create-itemcategories"></a><span data-ttu-id="4c841-103">Criar categorias de categoria</span><span class="sxs-lookup"><span data-stu-id="4c841-103">Create itemCategories</span></span>

<span data-ttu-id="4c841-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4c841-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c841-105">Criar um objeto de categoria de item Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4c841-105">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c841-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c841-106">Permissions</span></span>
<span data-ttu-id="4c841-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c841-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c841-109">Permission type</span></span> |<span data-ttu-id="4c841-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c841-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4c841-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c841-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c841-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c841-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4c841-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4c841-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4c841-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c841-114">Not supported.</span></span>|
|<span data-ttu-id="4c841-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c841-115">Application</span></span>|<span data-ttu-id="4c841-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c841-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c841-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c841-117">HTTP request</span></span>
```
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c841-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c841-118">Optional query parameters</span></span>
<span data-ttu-id="4c841-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c841-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c841-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c841-120">Request headers</span></span>
|<span data-ttu-id="4c841-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c841-121">Header</span></span>       |<span data-ttu-id="4c841-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c841-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="4c841-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c841-123">Authorization</span></span>|<span data-ttu-id="4c841-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c841-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c841-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c841-126">Content-Type</span></span> |<span data-ttu-id="4c841-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4c841-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="4c841-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c841-128">Request body</span></span>
<span data-ttu-id="4c841-129">No corpo da solicitação, forneça uma representação JSON de um objeto **myCategories** .</span><span class="sxs-lookup"><span data-stu-id="4c841-129">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="4c841-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c841-130">Response</span></span>
<span data-ttu-id="4c841-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **myCategories** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c841-131">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c841-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c841-132">Example</span></span>

<span data-ttu-id="4c841-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4c841-133">**Request**</span></span>

<span data-ttu-id="4c841-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c841-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="4c841-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="4c841-135">**Response**</span></span>

<span data-ttu-id="4c841-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c841-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="4c841-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c841-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c841-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c841-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




