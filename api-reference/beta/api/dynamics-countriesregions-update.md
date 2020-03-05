---
title: Atualizar countriesRegions
description: Atualiza um objeto de países/regiões no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a13eab313341bdc41f8a4bcbd023a5a32c3ca600
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431876"
---
# <a name="update-countriesregions"></a><span data-ttu-id="a2f51-103">Atualizar countriesRegions</span><span class="sxs-lookup"><span data-stu-id="a2f51-103">Update countriesRegions</span></span>

<span data-ttu-id="a2f51-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2f51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f51-105">Atualizar as propriedades de um objeto de país/região para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a2f51-105">Update the properties of a country/region object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2f51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2f51-106">Permissions</span></span>
<span data-ttu-id="a2f51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2f51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2f51-109">Permission type</span></span> |<span data-ttu-id="a2f51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2f51-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a2f51-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2f51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2f51-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f51-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a2f51-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2f51-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a2f51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2f51-114">Not supported.</span></span>|
|<span data-ttu-id="a2f51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2f51-115">Application</span></span>|<span data-ttu-id="a2f51-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f51-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2f51-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f51-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/countriesRegions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2f51-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2f51-118">Optional query parameters</span></span>
<span data-ttu-id="a2f51-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f51-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2f51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f51-120">Request headers</span></span>
|<span data-ttu-id="a2f51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2f51-121">Header</span></span>|<span data-ttu-id="a2f51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a2f51-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a2f51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2f51-123">Authorization</span></span> |<span data-ttu-id="a2f51-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2f51-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a2f51-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2f51-126">Content-Type</span></span>  |<span data-ttu-id="a2f51-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a2f51-127">application/json</span></span>|
|<span data-ttu-id="a2f51-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="a2f51-128">If-Match</span></span>      |<span data-ttu-id="a2f51-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2f51-129">Required.</span></span> <span data-ttu-id="a2f51-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **countriesRegions**, o **countriesRegions** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="a2f51-130">When this request header is included and the eTag provided does not match the current tag on the **countriesRegions**, the **countriesRegions** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2f51-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f51-131">Request body</span></span>
<span data-ttu-id="a2f51-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a2f51-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a2f51-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2f51-135">Response</span></span>
<span data-ttu-id="a2f51-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **countriesRegions** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f51-136">If successful, this method returns a `200 OK` response code and an updated **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2f51-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2f51-137">Example</span></span>

<span data-ttu-id="a2f51-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a2f51-138">**Request**</span></span>

<span data-ttu-id="a2f51-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2f51-139">Here is an example of the request.</span></span>

```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/countriesRegions/{id}
Content-type: application/json

{
  "displayName": "United States of America"
}
```

<span data-ttu-id="a2f51-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="a2f51-140">**Response**</span></span>

<span data-ttu-id="a2f51-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f51-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="a2f51-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a2f51-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a2f51-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2f51-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States of America",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-16T15:22:31.753Z"
}
```
