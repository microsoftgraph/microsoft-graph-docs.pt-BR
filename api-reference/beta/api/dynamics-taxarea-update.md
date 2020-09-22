---
title: Atualizar taxAreas
description: Atualiza um objeto de áreas de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f1918c8fa5a73672c06b824958d6d3cfa5ef0f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008089"
---
# <a name="update-taxareas"></a><span data-ttu-id="2a7f3-103">Atualizar taxAreas</span><span class="sxs-lookup"><span data-stu-id="2a7f3-103">Update taxAreas</span></span>

<span data-ttu-id="2a7f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a7f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a7f3-105">Atualizar as propriedades de um objeto de área de impostos para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-105">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a7f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a7f3-106">Permissions</span></span>
<span data-ttu-id="2a7f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a7f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a7f3-109">Permission type</span></span> |<span data-ttu-id="2a7f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a7f3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2a7f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a7f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7f3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a7f3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2a7f3-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2a7f3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2a7f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-114">Not supported.</span></span>|
|<span data-ttu-id="2a7f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a7f3-115">Application</span></span>|<span data-ttu-id="2a7f3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a7f3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a7f3-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a7f3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a7f3-118">Optional query parameters</span></span>
<span data-ttu-id="2a7f3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a7f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a7f3-120">Request headers</span></span>
|<span data-ttu-id="2a7f3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a7f3-121">Header</span></span>|<span data-ttu-id="2a7f3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a7f3-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="2a7f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a7f3-123">Authorization</span></span> |<span data-ttu-id="2a7f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a7f3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a7f3-126">Content-Type</span></span>  |<span data-ttu-id="2a7f3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a7f3-127">application/json</span></span>|
|<span data-ttu-id="2a7f3-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="2a7f3-128">If-Match</span></span>      |<span data-ttu-id="2a7f3-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-129">Required.</span></span> <span data-ttu-id="2a7f3-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **taxAreas**, o **taxAreas** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-130">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a7f3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a7f3-131">Request body</span></span>
<span data-ttu-id="2a7f3-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="2a7f3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a7f3-135">Response</span></span>
<span data-ttu-id="2a7f3-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **taxAreas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-136">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a7f3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a7f3-137">Example</span></span>

<span data-ttu-id="2a7f3-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="2a7f3-138">**Request**</span></span>

<span data-ttu-id="2a7f3-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="2a7f3-140">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="2a7f3-140">**Response**</span></span>

<span data-ttu-id="2a7f3-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="2a7f3-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2a7f3-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a7f3-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



