---
title: Atualizar customerPayments
description: Atualiza um objeto de pagamento de cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3fd77f188331376582c07edb1e60241edecb0337
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981433"
---
# <a name="update-customerpayments"></a><span data-ttu-id="096b4-103">Atualizar customerPayments</span><span class="sxs-lookup"><span data-stu-id="096b4-103">Update customerPayments</span></span>

<span data-ttu-id="096b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="096b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="096b4-105">Atualizar as propriedades de um objeto de pagamento de cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="096b4-105">Update the properties of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="096b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="096b4-106">Permissions</span></span>
<span data-ttu-id="096b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="096b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="096b4-109">Permission type</span></span> |<span data-ttu-id="096b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="096b4-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="096b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="096b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="096b4-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096b4-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="096b4-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="096b4-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="096b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="096b4-114">Not supported.</span></span>|
|<span data-ttu-id="096b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="096b4-115">Application</span></span>|<span data-ttu-id="096b4-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096b4-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="096b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="096b4-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="096b4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="096b4-118">Optional query parameters</span></span>
<span data-ttu-id="096b4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="096b4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="096b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="096b4-120">Request headers</span></span>
|<span data-ttu-id="096b4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="096b4-121">Header</span></span>        |<span data-ttu-id="096b4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="096b4-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="096b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="096b4-123">Authorization</span></span> |<span data-ttu-id="096b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="096b4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="096b4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="096b4-126">Content-Type</span></span>  |<span data-ttu-id="096b4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="096b4-127">application/json</span></span>         |
|<span data-ttu-id="096b4-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="096b4-128">If-Match</span></span>      |<span data-ttu-id="096b4-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="096b4-129">Required.</span></span> <span data-ttu-id="096b4-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **customerPayments**, o **customerPayments** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="096b4-130">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span>    |

## <a name="request-body"></a><span data-ttu-id="096b4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="096b4-131">Request body</span></span>
<span data-ttu-id="096b4-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="096b4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="096b4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="096b4-135">Response</span></span>
<span data-ttu-id="096b4-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **customerPayments** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="096b4-136">If successful, this method returns a `200 OK` response code and an updated **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="096b4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="096b4-137">Example</span></span>

<span data-ttu-id="096b4-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="096b4-138">**Request**</span></span>

<span data-ttu-id="096b4-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="096b4-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="096b4-140">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="096b4-140">**Response**</span></span>

<span data-ttu-id="096b4-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="096b4-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="096b4-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="096b4-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="096b4-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="096b4-143">All the properties will be returned from an actual call.</span></span>

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



