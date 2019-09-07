---
title: Obter customerPayments
description: Obtém um objeto de pagamento de cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2cf941f8efe1f00ebe5787ef5235501f65e90843
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791740"
---
# <a name="get-customerpayments"></a><span data-ttu-id="4036d-103">Obter customerPayments</span><span class="sxs-lookup"><span data-stu-id="4036d-103">Get customerPayments</span></span>
<span data-ttu-id="4036d-104">Recupere as propriedades e os relacionamentos de um objeto de pagamento de cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4036d-104">Retrieve the properties and relationships of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4036d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4036d-105">Permissions</span></span>
<span data-ttu-id="4036d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4036d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4036d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4036d-108">Permission type</span></span> |<span data-ttu-id="4036d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4036d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4036d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4036d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4036d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4036d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4036d-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4036d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4036d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4036d-113">Not supported.</span></span>|
|<span data-ttu-id="4036d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4036d-114">Application</span></span>|<span data-ttu-id="4036d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4036d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4036d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4036d-116">HTTP request</span></span>

```
GET /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4036d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4036d-117">Optional query parameters</span></span>
<span data-ttu-id="4036d-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4036d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4036d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4036d-119">Request headers</span></span>
|<span data-ttu-id="4036d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4036d-120">Header</span></span>|<span data-ttu-id="4036d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4036d-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="4036d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4036d-122">Authorization</span></span>  |<span data-ttu-id="4036d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4036d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4036d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4036d-125">Request body</span></span>
<span data-ttu-id="4036d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4036d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4036d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4036d-127">Response</span></span>
<span data-ttu-id="4036d-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPayments** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4036d-128">If successful, this method returns a `200 OK` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4036d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4036d-129">Example</span></span>

<span data-ttu-id="4036d-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4036d-130">**Request**</span></span>

<span data-ttu-id="4036d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4036d-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

<span data-ttu-id="4036d-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="4036d-132">**Response**</span></span>

<span data-ttu-id="4036d-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4036d-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="4036d-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4036d-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4036d-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4036d-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "journalDisplayName": "GENERAL",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "string",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

