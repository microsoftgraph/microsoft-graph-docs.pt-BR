---
title: Atualizar unitsOfMeasure
description: Atualiza uma unidade de objeto measure no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2dbaab40ef021024535591a33c76af56f8fe0642
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044827"
---
# <a name="update-unitsofmeasure"></a><span data-ttu-id="1b78f-103">Atualizar unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="1b78f-103">Update unitsOfMeasure</span></span>

<span data-ttu-id="1b78f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b78f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b78f-105">Atualize as propriedades de uma unidade de objeto measure para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1b78f-105">Update the properties of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b78f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b78f-106">Permissions</span></span>
<span data-ttu-id="1b78f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b78f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b78f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b78f-109">Permission type</span></span> |<span data-ttu-id="1b78f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b78f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1b78f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b78f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b78f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b78f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1b78f-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b78f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1b78f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b78f-114">Not supported.</span></span>|
|<span data-ttu-id="1b78f-115">Application</span><span class="sxs-lookup"><span data-stu-id="1b78f-115">Application</span></span>|<span data-ttu-id="1b78f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b78f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b78f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b78f-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b78f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b78f-118">Optional query parameters</span></span>
<span data-ttu-id="1b78f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b78f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b78f-120">Request headers</span></span>
|<span data-ttu-id="1b78f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b78f-121">Header</span></span>|<span data-ttu-id="1b78f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b78f-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="1b78f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b78f-123">Authorization</span></span> |<span data-ttu-id="1b78f-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="1b78f-124">Bearer.</span></span> <span data-ttu-id="1b78f-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b78f-125">Required.</span></span>|
|<span data-ttu-id="1b78f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b78f-126">Content-Type</span></span>  |<span data-ttu-id="1b78f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1b78f-127">application/json</span></span>|
|<span data-ttu-id="1b78f-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="1b78f-128">If-Match</span></span>      |<span data-ttu-id="1b78f-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b78f-129">Required.</span></span> <span data-ttu-id="1b78f-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual em **unitsOfMeasure**, **as unidadesOfMeasure** não serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="1b78f-130">When this request header is included and the eTag provided does not match the current tag on the **unitsOfMeasure**, the **unitsOfMeasure** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b78f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b78f-131">Request body</span></span>
<span data-ttu-id="1b78f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1b78f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="1b78f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b78f-135">Response</span></span>
<span data-ttu-id="1b78f-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto **unitsOfMeasure** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78f-136">If successful, this method returns a `200 OK` response code and an updated **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b78f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b78f-137">Example</span></span>

<span data-ttu-id="1b78f-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1b78f-138">**Request**</span></span>

<span data-ttu-id="1b78f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b78f-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
Content-type: application/json

{
  "displayName": "One Piece"
}
```

<span data-ttu-id="1b78f-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="1b78f-140">**Response**</span></span>

<span data-ttu-id="1b78f-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78f-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="1b78f-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b78f-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "One Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```



