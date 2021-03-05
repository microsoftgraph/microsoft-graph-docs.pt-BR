---
title: Obter companyInformation
description: Obtém um objeto de informações da empresa no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: fcbba1e491df93040865f5720e88c04ebe06af9c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473669"
---
# <a name="get-companyinformation"></a><span data-ttu-id="cfd69-103">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="cfd69-103">Get companyInformation</span></span>

<span data-ttu-id="cfd69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfd69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfd69-105">Recupere as propriedades e as relações de um objeto de informações da empresa para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="cfd69-105">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfd69-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfd69-106">Permissions</span></span>
<span data-ttu-id="cfd69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfd69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfd69-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfd69-109">Permission type</span></span> |<span data-ttu-id="cfd69-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfd69-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cfd69-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfd69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cfd69-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd69-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cfd69-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cfd69-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cfd69-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfd69-114">Not supported.</span></span>|
|<span data-ttu-id="cfd69-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfd69-115">Application</span></span>|<span data-ttu-id="cfd69-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd69-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfd69-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfd69-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/companyInformation/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cfd69-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cfd69-118">Optional query parameters</span></span>
<span data-ttu-id="cfd69-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cfd69-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfd69-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfd69-120">Request headers</span></span>
|<span data-ttu-id="cfd69-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfd69-121">Header</span></span>|<span data-ttu-id="cfd69-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfd69-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="cfd69-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfd69-123">Authorization</span></span>  |<span data-ttu-id="cfd69-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfd69-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfd69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfd69-126">Request body</span></span>
<span data-ttu-id="cfd69-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfd69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfd69-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfd69-128">Response</span></span>
<span data-ttu-id="cfd69-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **companyInformation** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfd69-129">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfd69-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfd69-130">Example</span></span>

<span data-ttu-id="cfd69-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="cfd69-131">**Request**</span></span>

<span data-ttu-id="cfd69-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfd69-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
```

<span data-ttu-id="cfd69-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="cfd69-133">**Response**</span></span>

<span data-ttu-id="cfd69-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfd69-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="cfd69-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfd69-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cfd69-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfd69-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "displayName": "CRONUS USA, Inc.",
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
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/companyInformation/{id}/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```


