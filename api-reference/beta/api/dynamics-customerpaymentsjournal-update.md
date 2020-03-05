---
title: Atualizar customerPaymentJournals
description: Atualiza um diário de pagamento do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4b0bd67fd8e0af4828bcdae920103d44a660c776
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430501"
---
# <a name="update-customerpaymentjournals"></a><span data-ttu-id="b8291-103">Atualizar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="b8291-103">Update customerPaymentJournals</span></span>

<span data-ttu-id="b8291-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b8291-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8291-105">Atualizar as propriedades de um objeto de diário de pagamentos do cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b8291-105">Update the properties of a customer payments journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8291-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8291-106">Permissions</span></span>
<span data-ttu-id="b8291-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8291-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8291-109">Permission type</span></span> |<span data-ttu-id="b8291-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8291-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b8291-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8291-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8291-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8291-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b8291-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b8291-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b8291-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8291-114">Not supported.</span></span>|
|<span data-ttu-id="b8291-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8291-115">Application</span></span>|<span data-ttu-id="b8291-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8291-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8291-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8291-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8291-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8291-118">Optional query parameters</span></span>
<span data-ttu-id="b8291-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8291-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8291-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8291-120">Request headers</span></span>
|<span data-ttu-id="b8291-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8291-121">Header</span></span>|<span data-ttu-id="b8291-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8291-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="b8291-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8291-123">Authorization</span></span> |<span data-ttu-id="b8291-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8291-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b8291-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8291-126">Content-Type</span></span>  |<span data-ttu-id="b8291-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b8291-127">application/json</span></span>|
|<span data-ttu-id="b8291-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="b8291-128">If-Match</span></span>      |<span data-ttu-id="b8291-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8291-129">Required.</span></span> <span data-ttu-id="b8291-130">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **customerPaymentJournals**, o **customerPaymentJournals** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="b8291-130">When this request header is included and the eTag provided does not match the current tag on the **customerPaymentJournals**, the **customerPaymentJournals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8291-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8291-131">Request body</span></span>
<span data-ttu-id="b8291-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b8291-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b8291-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8291-135">Response</span></span>
<span data-ttu-id="b8291-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPaymentJournals** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8291-136">If successful, this method returns a `200 OK` response code and an updated **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8291-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8291-137">Example</span></span>

<span data-ttu-id="b8291-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b8291-138">**Request**</span></span>

<span data-ttu-id="b8291-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8291-139">Here is an example of the request.</span></span>

```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}
Content-type: application/json

{
  "code": "EXPENSE",
  "displayName": "Expense Batch"
}
```

<span data-ttu-id="b8291-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="b8291-140">**Response**</span></span>

<span data-ttu-id="b8291-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8291-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="b8291-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8291-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8291-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8291-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "EXPENSE",
  "displayName": "Expense Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

