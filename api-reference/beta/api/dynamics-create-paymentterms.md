---
title: Criar paymentTerms
description: Cria um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 40f39f94f0249e2fa9947d8b3f828fc344a1ed39
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791915"
---
# <a name="create-paymentterms"></a><span data-ttu-id="cdd04-103">Criar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="cdd04-103">Create paymentTerms</span></span>
<span data-ttu-id="cdd04-104">Criar um objeto de condições de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="cdd04-104">Create a payment terms object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd04-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdd04-105">Permissions</span></span>
<span data-ttu-id="cdd04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd04-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdd04-108">Permission type</span></span> |<span data-ttu-id="cdd04-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdd04-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cdd04-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdd04-110">Delegated (work or school account)</span></span>|<span data-ttu-id="cdd04-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd04-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cdd04-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cdd04-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cdd04-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdd04-113">Not supported.</span></span>|
|<span data-ttu-id="cdd04-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdd04-114">Application</span></span>|<span data-ttu-id="cdd04-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd04-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdd04-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd04-116">HTTP request</span></span>
```
POST /financials/companies/{id}/paymentTerms
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdd04-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cdd04-117">Optional query parameters</span></span>
<span data-ttu-id="cdd04-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd04-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdd04-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd04-119">Request headers</span></span>
|<span data-ttu-id="cdd04-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdd04-120">Header</span></span>|<span data-ttu-id="cdd04-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cdd04-121">Value</span></span>|
|---------------|-----------------------------|
|<span data-ttu-id="cdd04-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdd04-122">Authorization</span></span>  |<span data-ttu-id="cdd04-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdd04-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="cdd04-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdd04-125">Content-Type</span></span>   |<span data-ttu-id="cdd04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdd04-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="cdd04-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdd04-127">Request body</span></span>
<span data-ttu-id="cdd04-128">No corpo da solicitação, forneça uma representação JSON de um objeto **paymentTerms** .</span><span class="sxs-lookup"><span data-stu-id="cdd04-128">In the request body, supply a JSON representation of a **paymentTerms** object.</span></span>

## <a name="response"></a><span data-ttu-id="cdd04-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdd04-129">Response</span></span>
<span data-ttu-id="cdd04-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **paymentTerms** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd04-130">If successful, this method returns ```201 Created``` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdd04-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdd04-131">Example</span></span>

<span data-ttu-id="cdd04-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="cdd04-132">**Request**</span></span>

<span data-ttu-id="cdd04-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdd04-133">Here is an example of a request.</span></span>

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

<span data-ttu-id="cdd04-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="cdd04-134">**Response**</span></span>

<span data-ttu-id="cdd04-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdd04-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="cdd04-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdd04-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cdd04-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdd04-137">All the properties will be returned from an actual call.</span></span>

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
