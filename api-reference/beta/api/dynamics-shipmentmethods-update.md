---
title: Atualizar shipmentMethods
description: Atualiza um objeto de método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 09790bc3983557a1e6f08210e44dd63f1068c475
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008194"
---
# <a name="update-shipmentmethods"></a><span data-ttu-id="ecbfa-103">Atualizar shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="ecbfa-103">Update shipmentMethods</span></span>

<span data-ttu-id="ecbfa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecbfa-105">Atualizar as propriedades de um objeto de método de remessa para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-105">Update the properties of a shipment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecbfa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecbfa-106">Permissions</span></span>
<span data-ttu-id="ecbfa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecbfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecbfa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecbfa-109">Permission type</span></span> |<span data-ttu-id="ecbfa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecbfa-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ecbfa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecbfa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecbfa-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbfa-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ecbfa-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ecbfa-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ecbfa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-114">Not supported.</span></span>|
|<span data-ttu-id="ecbfa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecbfa-115">Application</span></span>|<span data-ttu-id="ecbfa-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbfa-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecbfa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecbfa-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/shipmentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecbfa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecbfa-118">Optional query parameters</span></span>
<span data-ttu-id="ecbfa-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecbfa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecbfa-120">Request headers</span></span>
|<span data-ttu-id="ecbfa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecbfa-121">Header</span></span>|<span data-ttu-id="ecbfa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ecbfa-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="ecbfa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecbfa-123">Authorization</span></span> |<span data-ttu-id="ecbfa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ecbfa-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecbfa-126">Content-Type</span></span>  |<span data-ttu-id="ecbfa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ecbfa-127">application/json</span></span>|
|<span data-ttu-id="ecbfa-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="ecbfa-128">If-Match</span></span>      |<span data-ttu-id="ecbfa-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-129">Required.</span></span> <span data-ttu-id="ecbfa-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **shipmentMethods**, o **shipmentMethods** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-130">When this request header is included and the eTag provided does not match the current tag on the **shipmentMethods**, the **shipmentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecbfa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecbfa-131">Request body</span></span>
<span data-ttu-id="ecbfa-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ecbfa-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecbfa-135">Response</span></span>
<span data-ttu-id="ecbfa-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **shipmentMethods** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-136">If successful, this method returns a `200 OK` response code and an updated **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecbfa-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecbfa-137">Example</span></span>

<span data-ttu-id="ecbfa-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="ecbfa-138">**Request**</span></span>

<span data-ttu-id="ecbfa-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods/{id}
Content-type: application/json

{
  "displayName": "Pickup at Store Location"
}
```

<span data-ttu-id="ecbfa-140">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="ecbfa-140">**Response**</span></span>

<span data-ttu-id="ecbfa-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="ecbfa-142">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-142">**Note**:  The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ecbfa-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecbfa-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Store Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
  }
```



