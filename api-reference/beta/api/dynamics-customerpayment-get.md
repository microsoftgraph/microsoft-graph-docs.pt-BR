---
title: Obter customerPayments
description: Obtém um objeto de pagamento de cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 23fe46d0ec50b8f4b1a09cfbe4457a467e7d28dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458674"
---
# <a name="get-customerpayments"></a><span data-ttu-id="b8e39-103">Obter customerPayments</span><span class="sxs-lookup"><span data-stu-id="b8e39-103">Get customerPayments</span></span>
<span data-ttu-id="b8e39-104">Recupere as propriedades e os relacionamentos de um objeto de pagamento de cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b8e39-104">Retrieve the properties and relationships of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8e39-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8e39-105">Permissions</span></span>
<span data-ttu-id="b8e39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8e39-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8e39-108">Permission type</span></span> |<span data-ttu-id="b8e39-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8e39-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b8e39-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8e39-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b8e39-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e39-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b8e39-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b8e39-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b8e39-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8e39-113">Not supported.</span></span>|
|<span data-ttu-id="b8e39-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8e39-114">Application</span></span>|<span data-ttu-id="b8e39-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e39-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8e39-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e39-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8e39-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8e39-117">Optional query parameters</span></span>
<span data-ttu-id="b8e39-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e39-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8e39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e39-119">Request headers</span></span>
|<span data-ttu-id="b8e39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8e39-120">Header</span></span>|<span data-ttu-id="b8e39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b8e39-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="b8e39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8e39-122">Authorization</span></span>  |<span data-ttu-id="b8e39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8e39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8e39-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e39-125">Request body</span></span>
<span data-ttu-id="b8e39-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8e39-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8e39-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e39-127">Response</span></span>
<span data-ttu-id="b8e39-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPayments** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e39-128">If successful, this method returns a `200 OK` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e39-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8e39-129">Example</span></span>

<span data-ttu-id="b8e39-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b8e39-130">**Request**</span></span>

<span data-ttu-id="b8e39-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8e39-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

<span data-ttu-id="b8e39-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="b8e39-132">**Response**</span></span>

<span data-ttu-id="b8e39-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e39-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="b8e39-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8e39-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8e39-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8e39-135">All the properties will be returned from an actual call.</span></span>

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

