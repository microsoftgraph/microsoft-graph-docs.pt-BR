---
title: Atualizar paymentMethods
description: Atualiza um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 95e9fc2e0de68f737bc68c51e16d55caaa573208
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956076"
---
# <a name="update-paymentmethods"></a><span data-ttu-id="fc1e1-103">Atualizar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="fc1e1-103">Update paymentMethods</span></span>
<span data-ttu-id="fc1e1-104">Atualizar as propriedades de um objeto de método de pagamento para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-104">Update the properties of a payment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc1e1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc1e1-105">Permissions</span></span>
<span data-ttu-id="fc1e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc1e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc1e1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc1e1-108">Permission type</span></span> |<span data-ttu-id="fc1e1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fc1e1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="fc1e1-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc1e1-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fc1e1-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="fc1e1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fc1e1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-113">Not supported.</span></span>|
|<span data-ttu-id="fc1e1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc1e1-114">Application</span></span>|<span data-ttu-id="fc1e1-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc1e1-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc1e1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc1e1-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/paymentMethods('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc1e1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc1e1-117">Optional query parameters</span></span>
<span data-ttu-id="fc1e1-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc1e1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc1e1-119">Request headers</span></span>
|<span data-ttu-id="fc1e1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc1e1-120">Header</span></span>        |<span data-ttu-id="fc1e1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc1e1-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="fc1e1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc1e1-122">Authorization</span></span> |<span data-ttu-id="fc1e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fc1e1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc1e1-125">Content-Type</span></span>  |<span data-ttu-id="fc1e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc1e1-126">application/json</span></span>          |
|<span data-ttu-id="fc1e1-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="fc1e1-127">If-Match</span></span>      |<span data-ttu-id="fc1e1-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-128">Required.</span></span> <span data-ttu-id="fc1e1-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **paymentMethods**, o **paymentMethods** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-129">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc1e1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc1e1-130">Request body</span></span>
<span data-ttu-id="fc1e1-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="fc1e1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc1e1-134">Response</span></span>
<span data-ttu-id="fc1e1-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **paymentMethods** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-135">If successful, this method returns a `200 OK` response code and an updated **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc1e1-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc1e1-136">Example</span></span>

<span data-ttu-id="fc1e1-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="fc1e1-137">**Request**</span></span>

<span data-ttu-id="fc1e1-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods('{id}')
Content-type: application/json

{
  "displayName": "Personal Check Payment",
}
```

<span data-ttu-id="fc1e1-139">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="fc1e1-139">**Response**</span></span>

<span data-ttu-id="fc1e1-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="fc1e1-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc1e1-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Personal Check Payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```


