---
title: Atualizar paymentTerms
description: Atualiza um objeto de termo de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3a7c596850989831c549f7cb642318e31f7fa420
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956020"
---
# <a name="update-paymentterms"></a><span data-ttu-id="9a397-103">Atualizar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="9a397-103">Update paymentTerms</span></span>
<span data-ttu-id="9a397-104">Atualizar as propriedades de um objeto de condições de pagamento para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="9a397-104">Update the properties of a payment terms object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a397-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a397-105">Permissions</span></span>
<span data-ttu-id="9a397-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a397-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a397-108">Permission type</span></span> |<span data-ttu-id="9a397-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a397-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9a397-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a397-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9a397-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a397-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9a397-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9a397-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9a397-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a397-113">Not supported.</span></span>|
|<span data-ttu-id="9a397-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a397-114">Application</span></span>|<span data-ttu-id="9a397-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a397-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a397-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a397-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/paymentTerms('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a397-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a397-117">Optional query parameters</span></span>
<span data-ttu-id="9a397-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a397-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a397-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a397-119">Request headers</span></span>
|<span data-ttu-id="9a397-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a397-120">Header</span></span>        |<span data-ttu-id="9a397-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9a397-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="9a397-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a397-122">Authorization</span></span> |<span data-ttu-id="9a397-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a397-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9a397-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a397-125">Content-Type</span></span>  |<span data-ttu-id="9a397-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a397-126">application/json</span></span>         |
|<span data-ttu-id="9a397-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="9a397-127">If-Match</span></span>      |<span data-ttu-id="9a397-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a397-128">Required.</span></span> <span data-ttu-id="9a397-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **paymentTerms**, o **paymentTerms** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="9a397-129">When this request header is included and the eTag provided does not match the current tag on the **paymentTerms**, the **paymentTerms** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a397-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a397-130">Request body</span></span>
<span data-ttu-id="9a397-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9a397-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="9a397-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a397-134">Response</span></span>
<span data-ttu-id="9a397-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **paymentTerms** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a397-135">If successful, this method returns a `200 OK` response code and an updated **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a397-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a397-136">Example</span></span>

<span data-ttu-id="9a397-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="9a397-137">**Request**</span></span>

<span data-ttu-id="9a397-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a397-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms('{id}')
Content-type: application/json

{
  "displayName": "Net 7 days with Discount",
  "discountPercent": 10
}
```

<span data-ttu-id="9a397-139">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="9a397-139">**Response**</span></span>

<span data-ttu-id="9a397-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a397-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="9a397-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a397-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a397-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a397-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days with Discount",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 10,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-15T02:20:55.203Z"
}
```

