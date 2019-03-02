---
title: Criar shipmentMethods
description: Cria um objeto de método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4f83c186adf72dde6f88082db1a6156ebc7b12af
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365812"
---
# <a name="create-shipmentmethods"></a><span data-ttu-id="f722d-103">Criar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f722d-103">Create shipmentMethods</span></span>
<span data-ttu-id="f722d-104">Criar um objeto de método de remessa no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f722d-104">Create a shipment method object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f722d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f722d-105">Permissions</span></span>
<span data-ttu-id="f722d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f722d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f722d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f722d-108">Permission type</span></span> |<span data-ttu-id="f722d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f722d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f722d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f722d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f722d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f722d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f722d-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f722d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f722d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f722d-113">Not supported.</span></span>|
|<span data-ttu-id="f722d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f722d-114">Application</span></span>|<span data-ttu-id="f722d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f722d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f722d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f722d-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/shipmentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f722d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f722d-117">Optional query parameters</span></span>
<span data-ttu-id="f722d-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f722d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f722d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f722d-119">Request headers</span></span>

|<span data-ttu-id="f722d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f722d-120">Header</span></span>         |<span data-ttu-id="f722d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f722d-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="f722d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f722d-122">Authorization</span></span>  |<span data-ttu-id="f722d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f722d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f722d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f722d-125">Content-Type</span></span>   |<span data-ttu-id="f722d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f722d-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="f722d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f722d-127">Request body</span></span>
<span data-ttu-id="f722d-128">No corpo da solicitação, forneça uma representação JSON de um objeto **shipmentMethods** .</span><span class="sxs-lookup"><span data-stu-id="f722d-128">In the request body, supply a JSON representation of a **shipmentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="f722d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f722d-129">Response</span></span>
<span data-ttu-id="f722d-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **shipmentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f722d-130">If successful, this method returns ```201 Created``` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f722d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f722d-131">Example</span></span>

<span data-ttu-id="f722d-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="f722d-132">**Request**</span></span>

<span data-ttu-id="f722d-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f722d-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

<span data-ttu-id="f722d-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="f722d-134">**Response**</span></span>

<span data-ttu-id="f722d-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f722d-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="f722d-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f722d-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f722d-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f722d-137">All the properties will be returned from an actual call.</span></span>

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
