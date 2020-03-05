---
title: Criar shipmentMethods
description: Cria um objeto de método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8b33d044549a67ce27bb160db382e06bbcf73b9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431250"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="59f2d-103">Criar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="59f2d-103">Create shipmentMethods</span></span>

<span data-ttu-id="59f2d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59f2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59f2d-105">Criar um objeto de método de remessa no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="59f2d-105">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="59f2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59f2d-106">Permissions</span></span>
<span data-ttu-id="59f2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59f2d-109">Permission type</span></span> |<span data-ttu-id="59f2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59f2d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="59f2d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59f2d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59f2d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f2d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="59f2d-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="59f2d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="59f2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59f2d-114">Not supported.</span></span>|
|<span data-ttu-id="59f2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59f2d-115">Application</span></span>|<span data-ttu-id="59f2d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f2d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59f2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f2d-117">HTTP request</span></span>
```
POST /financials/companies/{id}/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59f2d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59f2d-118">Optional query parameters</span></span>
<span data-ttu-id="59f2d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59f2d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59f2d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59f2d-120">Request headers</span></span>

|<span data-ttu-id="59f2d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59f2d-121">Header</span></span>         |<span data-ttu-id="59f2d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59f2d-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="59f2d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59f2d-123">Authorization</span></span>  |<span data-ttu-id="59f2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59f2d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="59f2d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59f2d-126">Content-Type</span></span>   |<span data-ttu-id="59f2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="59f2d-127">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="59f2d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f2d-128">Request body</span></span>
<span data-ttu-id="59f2d-129">No corpo da solicitação, forneça uma representação JSON de um objeto **shipmentMethods** .</span><span class="sxs-lookup"><span data-stu-id="59f2d-129">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="59f2d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f2d-130">Response</span></span>
<span data-ttu-id="59f2d-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **shipmentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f2d-131">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f2d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f2d-132">Example</span></span>

<span data-ttu-id="59f2d-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="59f2d-133">**Request**</span></span>

<span data-ttu-id="59f2d-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="59f2d-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="59f2d-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="59f2d-135">**Response**</span></span>

<span data-ttu-id="59f2d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f2d-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="59f2d-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59f2d-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59f2d-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59f2d-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
