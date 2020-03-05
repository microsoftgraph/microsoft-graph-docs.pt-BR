---
title: Obter paymentTerms
description: Obtém um objeto de termo de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c2351a88f88b216e9e3833dc719533b89732aeb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428576"
---
# <a name="get-paymentterms"></a><span data-ttu-id="4c666-103">Obter paymentTerms</span><span class="sxs-lookup"><span data-stu-id="4c666-103">Get paymentTerms</span></span>

<span data-ttu-id="4c666-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4c666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c666-105">Recupere as propriedades e os relacionamentos de um objeto de condições de pagamento para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4c666-105">Retrieve the properties and relationships of a payment terms object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c666-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c666-106">Permissions</span></span>
<span data-ttu-id="4c666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c666-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c666-109">Permission type</span></span> |<span data-ttu-id="4c666-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c666-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4c666-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c666-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c666-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c666-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4c666-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4c666-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4c666-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c666-114">Not supported.</span></span>|
|<span data-ttu-id="4c666-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c666-115">Application</span></span>|<span data-ttu-id="4c666-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c666-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c666-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c666-117">HTTP request</span></span>

```
GET /financials/companies/{id}/paymentTerms/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c666-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c666-118">Optional query parameters</span></span>
<span data-ttu-id="4c666-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c666-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c666-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c666-120">Request headers</span></span>
|<span data-ttu-id="4c666-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c666-121">Header</span></span>         |<span data-ttu-id="4c666-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c666-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="4c666-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c666-123">Authorization</span></span>  |<span data-ttu-id="4c666-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c666-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c666-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c666-126">Request body</span></span>
<span data-ttu-id="4c666-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c666-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c666-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c666-128">Response</span></span>
<span data-ttu-id="4c666-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **paymentTerms** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c666-129">If successful, this method returns a `200 OK` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c666-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c666-130">Example</span></span>

<span data-ttu-id="4c666-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4c666-131">**Request**</span></span>

<span data-ttu-id="4c666-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c666-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms/{id}
```

<span data-ttu-id="4c666-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="4c666-133">**Response**</span></span>

<span data-ttu-id="4c666-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c666-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="4c666-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c666-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c666-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c666-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-15T02:20:55.203Z"
}
```
