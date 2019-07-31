---
title: Criar customerPayments
description: Cria um objeto Customer Payment no Dynamics 365 Business central.
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 621fe92d598894589cf39cb0371830792560ae6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956706"
---
# <a name="create-customerpayments"></a><span data-ttu-id="6a16f-103">Criar customerPayments</span><span class="sxs-lookup"><span data-stu-id="6a16f-103">Create customerPayments</span></span>
<span data-ttu-id="6a16f-104">Cria um objeto Customer Payment no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="6a16f-104">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a16f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a16f-105">Permissions</span></span>
<span data-ttu-id="6a16f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a16f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a16f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a16f-108">Permission type</span></span> |<span data-ttu-id="6a16f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a16f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6a16f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a16f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6a16f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a16f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6a16f-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6a16f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6a16f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a16f-113">Not supported.</span></span>|
|<span data-ttu-id="6a16f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a16f-114">Application</span></span>|<span data-ttu-id="6a16f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a16f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a16f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a16f-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a16f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a16f-117">Optional query parameters</span></span>
<span data-ttu-id="6a16f-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a16f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a16f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a16f-119">Request headers</span></span>
|<span data-ttu-id="6a16f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a16f-120">Header</span></span>        |<span data-ttu-id="6a16f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a16f-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="6a16f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a16f-122">Authorization</span></span> |<span data-ttu-id="6a16f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a16f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6a16f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a16f-125">Content-Type</span></span>  |<span data-ttu-id="6a16f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a16f-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="6a16f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a16f-127">Request body</span></span>
<span data-ttu-id="6a16f-128">No corpo da solicitação, forneça uma representação JSON do objeto **customerPayments** .</span><span class="sxs-lookup"><span data-stu-id="6a16f-128">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="6a16f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a16f-129">Response</span></span>
<span data-ttu-id="6a16f-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **customerPayments** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a16f-130">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a16f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a16f-131">Example</span></span>

<span data-ttu-id="6a16f-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="6a16f-132">**Request**</span></span>

<span data-ttu-id="6a16f-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a16f-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournal('{id}')/customerPayments
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
<span data-ttu-id="6a16f-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="6a16f-134">**Response**</span></span>

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

