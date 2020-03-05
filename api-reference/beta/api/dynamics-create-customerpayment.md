---
title: Criar customerPayments
description: Cria um objeto Customer Payment no Dynamics 365 Business central.
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 613ad01feddc87941a6e6775195364e75ca4e57a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431673"
---
# <a name="create-customerpayments"></a><span data-ttu-id="12f2b-103">Criar customerPayments</span><span class="sxs-lookup"><span data-stu-id="12f2b-103">Create customerPayments</span></span>

<span data-ttu-id="12f2b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12f2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12f2b-105">Cria um objeto Customer Payment no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="12f2b-105">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="12f2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12f2b-106">Permissions</span></span>
<span data-ttu-id="12f2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12f2b-109">Permission type</span></span> |<span data-ttu-id="12f2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12f2b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="12f2b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12f2b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12f2b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f2b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="12f2b-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="12f2b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="12f2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12f2b-114">Not supported.</span></span>|
|<span data-ttu-id="12f2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12f2b-115">Application</span></span>|<span data-ttu-id="12f2b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f2b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12f2b-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12f2b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12f2b-118">Optional query parameters</span></span>
<span data-ttu-id="12f2b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12f2b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12f2b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12f2b-120">Request headers</span></span>
|<span data-ttu-id="12f2b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12f2b-121">Header</span></span>        |<span data-ttu-id="12f2b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12f2b-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="12f2b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12f2b-123">Authorization</span></span> |<span data-ttu-id="12f2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12f2b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12f2b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12f2b-126">Content-Type</span></span>  |<span data-ttu-id="12f2b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12f2b-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="12f2b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12f2b-128">Request body</span></span>
<span data-ttu-id="12f2b-129">No corpo da solicitação, forneça uma representação JSON do objeto **customerPayments** .</span><span class="sxs-lookup"><span data-stu-id="12f2b-129">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="12f2b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12f2b-130">Response</span></span>
<span data-ttu-id="12f2b-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **customerPayments** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12f2b-131">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f2b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12f2b-132">Example</span></span>

<span data-ttu-id="12f2b-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="12f2b-133">**Request**</span></span>

<span data-ttu-id="12f2b-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="12f2b-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournal/{id}/customerPayments
Content-type: application/json

{
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": -1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
}
```
<span data-ttu-id="12f2b-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="12f2b-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

