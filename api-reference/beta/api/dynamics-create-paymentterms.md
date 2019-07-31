---
title: Criar paymentTerms
description: Cria um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 84a756dc92819a2ab40b6bc24600af9c66f2004c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956594"
---
# <a name="create-paymentterms"></a><span data-ttu-id="998ac-103">Criar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="998ac-103">Create paymentTerms</span></span>
<span data-ttu-id="998ac-104">Criar um objeto de condições de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="998ac-104">Create a payment terms object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="998ac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="998ac-105">Permissions</span></span>
<span data-ttu-id="998ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="998ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="998ac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="998ac-108">Permission type</span></span> |<span data-ttu-id="998ac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="998ac-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="998ac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="998ac-110">Delegated (work or school account)</span></span>|<span data-ttu-id="998ac-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="998ac-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="998ac-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="998ac-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="998ac-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="998ac-113">Not supported.</span></span>|
|<span data-ttu-id="998ac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="998ac-114">Application</span></span>|<span data-ttu-id="998ac-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="998ac-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="998ac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="998ac-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/paymentTerms
```

## <a name="optional-query-parameters"></a><span data-ttu-id="998ac-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="998ac-117">Optional query parameters</span></span>
<span data-ttu-id="998ac-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="998ac-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="998ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="998ac-119">Request headers</span></span>
|<span data-ttu-id="998ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="998ac-120">Header</span></span>|<span data-ttu-id="998ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="998ac-121">Value</span></span>|
|---------------|-----------------------------|
|<span data-ttu-id="998ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="998ac-122">Authorization</span></span>  |<span data-ttu-id="998ac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="998ac-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="998ac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="998ac-125">Content-Type</span></span>   |<span data-ttu-id="998ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="998ac-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="998ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="998ac-127">Request body</span></span>
<span data-ttu-id="998ac-128">No corpo da solicitação, forneça uma representação JSON de um objeto **paymentTerms** .</span><span class="sxs-lookup"><span data-stu-id="998ac-128">In the request body, supply a JSON representation of a **paymentTerms** object.</span></span>

## <a name="response"></a><span data-ttu-id="998ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="998ac-129">Response</span></span>
<span data-ttu-id="998ac-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **paymentTerms** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="998ac-130">If successful, this method returns ```201 Created``` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="998ac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="998ac-131">Example</span></span>

<span data-ttu-id="998ac-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="998ac-132">**Request**</span></span>

<span data-ttu-id="998ac-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="998ac-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms
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

<span data-ttu-id="998ac-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="998ac-134">**Response**</span></span>

<span data-ttu-id="998ac-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="998ac-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="998ac-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="998ac-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="998ac-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="998ac-137">All the properties will be returned from an actual call.</span></span>

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
