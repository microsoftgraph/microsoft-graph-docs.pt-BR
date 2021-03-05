---
title: Atualizar companyInformation
description: Atualiza um objeto de informações da empresa no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: eb94bf97caa58724286f464416884a179a1e1023
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473410"
---
# <a name="update-companyinformation"></a><span data-ttu-id="ad86a-103">Atualizar companyInformation</span><span class="sxs-lookup"><span data-stu-id="ad86a-103">Update companyInformation</span></span>

<span data-ttu-id="ad86a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad86a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad86a-105">Atualize as propriedades de um objeto de informações da empresa para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ad86a-105">Update the properties of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad86a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad86a-106">Permissions</span></span>
<span data-ttu-id="ad86a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad86a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad86a-109">Permission type</span></span> |<span data-ttu-id="ad86a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad86a-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ad86a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad86a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad86a-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad86a-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ad86a-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad86a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ad86a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad86a-114">Not supported.</span></span>|
|<span data-ttu-id="ad86a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad86a-115">Application</span></span>|<span data-ttu-id="ad86a-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad86a-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad86a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad86a-117">HTTP request</span></span>
```http
PATCH /financials/companies/{id}/companyInformation/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad86a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad86a-118">Optional query parameters</span></span>
<span data-ttu-id="ad86a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad86a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad86a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad86a-120">Request headers</span></span>
|<span data-ttu-id="ad86a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad86a-121">Header</span></span>        |<span data-ttu-id="ad86a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ad86a-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="ad86a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad86a-123">Authorization</span></span> |<span data-ttu-id="ad86a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad86a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad86a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad86a-126">Content-Type</span></span>  |<span data-ttu-id="ad86a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ad86a-127">application/json</span></span>         |
|<span data-ttu-id="ad86a-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="ad86a-128">If-Match</span></span>      |<span data-ttu-id="ad86a-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad86a-129">Required.</span></span> <span data-ttu-id="ad86a-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual na **companyInformation**, **a companyInformation** não será atualizada.</span><span class="sxs-lookup"><span data-stu-id="ad86a-130">When this request header is included and the eTag provided does not match the current tag on the **companyInformation**, the **companyInformation** will not be updated.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad86a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad86a-131">Request body</span></span>
<span data-ttu-id="ad86a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ad86a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ad86a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad86a-135">Response</span></span>
<span data-ttu-id="ad86a-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto **companyInformation** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad86a-136">If successful, this method returns a `200 OK` response code and an updated an **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad86a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad86a-137">Example</span></span>

<span data-ttu-id="ad86a-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="ad86a-138">**Request**</span></span>

<span data-ttu-id="ad86a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad86a-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
Content-type: application/json

{
  "displayName": "CRONUS USA, LTD.",
  "website": "www.cronuscorp.net"
}
```

<span data-ttu-id="ad86a-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="ad86a-140">**Response**</span></span>

<span data-ttu-id="ad86a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad86a-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="ad86a-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ad86a-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad86a-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad86a-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "displayName": "CRONUS USA, LTD.",
  "address": {
    "street": "7122 South Ashford Street\r\nWestminster",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "+1 425 555 0100",
  "faxNumber": "+1 425 555 0101",
  "email": "",
  "website": "www.cronuscorp.net",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/companyInformation/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
  }
```


