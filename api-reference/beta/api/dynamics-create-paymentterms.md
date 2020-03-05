---
title: Criar paymentTerms
description: Cria um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6d604f11bb5300e659102ec6301c7b6509d1244b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431320"
---
# <a name="create-paymentterms"></a><span data-ttu-id="65a76-103">Criar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="65a76-103">Create paymentTerms</span></span>

<span data-ttu-id="65a76-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65a76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65a76-105">Criar um objeto de condições de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="65a76-105">Create a payment terms object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="65a76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65a76-106">Permissions</span></span>
<span data-ttu-id="65a76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65a76-109">Permission type</span></span> |<span data-ttu-id="65a76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65a76-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="65a76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65a76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65a76-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a76-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="65a76-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="65a76-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="65a76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65a76-114">Not supported.</span></span>|
|<span data-ttu-id="65a76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65a76-115">Application</span></span>|<span data-ttu-id="65a76-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a76-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65a76-117">HTTP request</span></span>
```
POST /financials/companies/{id}/paymentTerms
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65a76-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65a76-118">Optional query parameters</span></span>
<span data-ttu-id="65a76-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65a76-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65a76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65a76-120">Request headers</span></span>
|<span data-ttu-id="65a76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65a76-121">Header</span></span>|<span data-ttu-id="65a76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="65a76-122">Value</span></span>|
|---------------|-----------------------------|
|<span data-ttu-id="65a76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="65a76-123">Authorization</span></span>  |<span data-ttu-id="65a76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65a76-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="65a76-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65a76-126">Content-Type</span></span>   |<span data-ttu-id="65a76-127">application/json</span><span class="sxs-lookup"><span data-stu-id="65a76-127">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="65a76-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65a76-128">Request body</span></span>
<span data-ttu-id="65a76-129">No corpo da solicitação, forneça uma representação JSON de um objeto **paymentTerms** .</span><span class="sxs-lookup"><span data-stu-id="65a76-129">In the request body, supply a JSON representation of a **paymentTerms** object.</span></span>

## <a name="response"></a><span data-ttu-id="65a76-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="65a76-130">Response</span></span>
<span data-ttu-id="65a76-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **paymentTerms** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a76-131">If successful, this method returns ```201 Created``` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a76-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65a76-132">Example</span></span>

<span data-ttu-id="65a76-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="65a76-133">**Request**</span></span>

<span data-ttu-id="65a76-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="65a76-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms
Content-type: application/json

{
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false
}
```

<span data-ttu-id="65a76-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="65a76-135">**Response**</span></span>

<span data-ttu-id="65a76-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a76-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="65a76-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65a76-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65a76-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65a76-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-03T02:14:32Z"
}

```
