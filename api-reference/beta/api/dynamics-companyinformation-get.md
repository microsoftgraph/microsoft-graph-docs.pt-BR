---
title: Obter companyInformation
description: Obtém um objeto de informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 10b8fff983f9c4f90bb40127ee5094a0fd0bdf74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956818"
---
# <a name="get-companyinformation"></a><span data-ttu-id="d13ae-103">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="d13ae-103">Get companyInformation</span></span>
<span data-ttu-id="d13ae-104">Recupere as propriedades e os relacionamentos de um objeto de informações da empresa para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="d13ae-104">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d13ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d13ae-105">Permissions</span></span>
<span data-ttu-id="d13ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d13ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d13ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d13ae-108">Permission type</span></span> |<span data-ttu-id="d13ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d13ae-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d13ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d13ae-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d13ae-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13ae-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d13ae-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d13ae-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d13ae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d13ae-113">Not supported.</span></span>|
|<span data-ttu-id="d13ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d13ae-114">Application</span></span>|<span data-ttu-id="d13ae-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13ae-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d13ae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d13ae-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/companyInformation('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d13ae-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d13ae-117">Optional query parameters</span></span>
<span data-ttu-id="d13ae-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d13ae-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d13ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d13ae-119">Request headers</span></span>
|<span data-ttu-id="d13ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d13ae-120">Header</span></span>|<span data-ttu-id="d13ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d13ae-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="d13ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d13ae-122">Authorization</span></span>  |<span data-ttu-id="d13ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d13ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d13ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d13ae-125">Request body</span></span>
<span data-ttu-id="d13ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d13ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d13ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13ae-127">Response</span></span>
<span data-ttu-id="d13ae-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **companyInformation** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d13ae-128">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d13ae-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d13ae-129">Example</span></span>

<span data-ttu-id="d13ae-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="d13ae-130">**Request**</span></span>

<span data-ttu-id="d13ae-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d13ae-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
```

<span data-ttu-id="d13ae-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="d13ae-132">**Response**</span></span>

<span data-ttu-id="d13ae-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d13ae-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="d13ae-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d13ae-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d13ae-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d13ae-135">All the properties will be returned from an actual call.</span></span>

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
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```
