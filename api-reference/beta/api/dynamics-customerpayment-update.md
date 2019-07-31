---
title: Atualizar customerPayments
description: Atualiza um objeto de pagamento de cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 120bf407ac38ffb5b2a4802905f4ae02ee134483
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956398"
---
# <a name="update-customerpayments"></a><span data-ttu-id="daed9-103">Atualizar customerPayments</span><span class="sxs-lookup"><span data-stu-id="daed9-103">Update customerPayments</span></span>
<span data-ttu-id="daed9-104">Atualizar as propriedades de um objeto de pagamento de cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="daed9-104">Update the properties of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="daed9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="daed9-105">Permissions</span></span>
<span data-ttu-id="daed9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daed9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daed9-108">Permission type</span></span> |<span data-ttu-id="daed9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="daed9-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="daed9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daed9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="daed9-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daed9-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="daed9-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="daed9-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="daed9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daed9-113">Not supported.</span></span>|
|<span data-ttu-id="daed9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daed9-114">Application</span></span>|<span data-ttu-id="daed9-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daed9-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daed9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daed9-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daed9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="daed9-117">Optional query parameters</span></span>
<span data-ttu-id="daed9-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="daed9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="daed9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daed9-119">Request headers</span></span>
|<span data-ttu-id="daed9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daed9-120">Header</span></span>        |<span data-ttu-id="daed9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="daed9-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="daed9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="daed9-122">Authorization</span></span> |<span data-ttu-id="daed9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daed9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="daed9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daed9-125">Content-Type</span></span>  |<span data-ttu-id="daed9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daed9-126">application/json</span></span>         |
|<span data-ttu-id="daed9-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="daed9-127">If-Match</span></span>      |<span data-ttu-id="daed9-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daed9-128">Required.</span></span> <span data-ttu-id="daed9-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **customerPayments**, o **customerPayments** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="daed9-129">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span>    |

## <a name="request-body"></a><span data-ttu-id="daed9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daed9-130">Request body</span></span>
<span data-ttu-id="daed9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="daed9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="daed9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="daed9-134">Response</span></span>
<span data-ttu-id="daed9-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPayments** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daed9-135">If successful, this method returns a `200 OK` response code and an updated **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daed9-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daed9-136">Example</span></span>

<span data-ttu-id="daed9-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="daed9-137">**Request**</span></span>

<span data-ttu-id="daed9-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daed9-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="daed9-139">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="daed9-139">**Response**</span></span>

<span data-ttu-id="daed9-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daed9-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="daed9-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="daed9-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="daed9-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daed9-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": -2000,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

