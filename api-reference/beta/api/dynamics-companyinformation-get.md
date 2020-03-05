---
title: Obter companyInformation
description: Obtém um objeto de informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ef94284b3c543868987a82a0f8422e9018060bdd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431960"
---
# <a name="get-companyinformation"></a><span data-ttu-id="87a16-103">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="87a16-103">Get companyInformation</span></span>

<span data-ttu-id="87a16-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87a16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87a16-105">Recupere as propriedades e os relacionamentos de um objeto de informações da empresa para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="87a16-105">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="87a16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87a16-106">Permissions</span></span>
<span data-ttu-id="87a16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87a16-109">Permission type</span></span> |<span data-ttu-id="87a16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87a16-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="87a16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87a16-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87a16-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a16-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="87a16-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="87a16-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="87a16-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a16-114">Not supported.</span></span>|
|<span data-ttu-id="87a16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87a16-115">Application</span></span>|<span data-ttu-id="87a16-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a16-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87a16-117">HTTP request</span></span>
```
GET /financials/companies/{id}/companyInformation/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87a16-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87a16-118">Optional query parameters</span></span>
<span data-ttu-id="87a16-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87a16-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87a16-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87a16-120">Request headers</span></span>
|<span data-ttu-id="87a16-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87a16-121">Header</span></span>|<span data-ttu-id="87a16-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87a16-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="87a16-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87a16-123">Authorization</span></span>  |<span data-ttu-id="87a16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87a16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87a16-126">Request body</span></span>
<span data-ttu-id="87a16-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87a16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87a16-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a16-128">Response</span></span>
<span data-ttu-id="87a16-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **companyInformation** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a16-129">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a16-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87a16-130">Example</span></span>

<span data-ttu-id="87a16-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="87a16-131">**Request**</span></span>

<span data-ttu-id="87a16-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87a16-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
```

<span data-ttu-id="87a16-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="87a16-133">**Response**</span></span>

<span data-ttu-id="87a16-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a16-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="87a16-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="87a16-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="87a16-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87a16-136">All the properties will be returned from an actual call.</span></span>

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
