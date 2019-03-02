---
title: Atualizar diários
description: Atualiza um objeto Journal no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 5c5614a84852e81977cdf443543364507544bd27
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365854"
---
# <a name="update-journals"></a><span data-ttu-id="184ad-103">Atualizar diários</span><span class="sxs-lookup"><span data-stu-id="184ad-103">Update journals</span></span>
<span data-ttu-id="184ad-104">Atualizar as propriedades de um objeto Journal para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="184ad-104">Update the properties of a journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="184ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="184ad-105">Permissions</span></span>
<span data-ttu-id="184ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="184ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="184ad-108">Permission type</span></span> |<span data-ttu-id="184ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="184ad-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="184ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="184ad-110">Delegated (work or school account)</span></span>|<span data-ttu-id="184ad-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184ad-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="184ad-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="184ad-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="184ad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184ad-113">Not supported.</span></span>|
|<span data-ttu-id="184ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="184ad-114">Application</span></span>|<span data-ttu-id="184ad-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184ad-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="184ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="184ad-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="184ad-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="184ad-117">Optional query parameters</span></span>
<span data-ttu-id="184ad-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="184ad-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="184ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="184ad-119">Request headers</span></span>
|<span data-ttu-id="184ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="184ad-120">Header</span></span>        |<span data-ttu-id="184ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="184ad-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="184ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="184ad-122">Authorization</span></span> |<span data-ttu-id="184ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184ad-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="184ad-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="184ad-125">Content-Type</span></span>  |<span data-ttu-id="184ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="184ad-126">application/json</span></span>         |
|<span data-ttu-id="184ad-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="184ad-127">If-Match</span></span>      |<span data-ttu-id="184ad-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184ad-128">Required.</span></span> <span data-ttu-id="184ad-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual dos **diários**, os **diários** não serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="184ad-129">When this request header is included and the eTag provided does not match the current tag on the **journals**, the **journals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="184ad-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="184ad-130">Request body</span></span>
<span data-ttu-id="184ad-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="184ad-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="184ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="184ad-134">Response</span></span>
<span data-ttu-id="184ad-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Journals** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="184ad-135">If successful, this method returns a `200 OK` response code and an updated **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="184ad-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="184ad-136">Example</span></span>

<span data-ttu-id="184ad-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="184ad-137">**Request**</span></span>

<span data-ttu-id="184ad-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="184ad-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')
Content-type: application/json

{
  "code": "EXPENSE",
  "displayName": "Expense Batch"
}
```

<span data-ttu-id="184ad-139">**Response**</span><span class="sxs-lookup"><span data-stu-id="184ad-139">**Response**</span></span>

<span data-ttu-id="184ad-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="184ad-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="184ad-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="184ad-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="184ad-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="184ad-142">All the properties will be returned from an actual call.</span></span>

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

