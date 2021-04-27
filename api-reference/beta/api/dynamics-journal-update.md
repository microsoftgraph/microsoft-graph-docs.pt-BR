---
title: Atualizar diários
description: Atualiza um objeto de diário no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a86533bd740a301724dd4098587959fc6bab5ce4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045198"
---
# <a name="update-journals"></a><span data-ttu-id="c26ea-103">Atualizar diários</span><span class="sxs-lookup"><span data-stu-id="c26ea-103">Update journals</span></span>

<span data-ttu-id="c26ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c26ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c26ea-105">Atualize as propriedades de um objeto de diário para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c26ea-105">Update the properties of a journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c26ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c26ea-106">Permissions</span></span>
<span data-ttu-id="c26ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c26ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c26ea-109">Permission type</span></span> |<span data-ttu-id="c26ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c26ea-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c26ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c26ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c26ea-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ea-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c26ea-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c26ea-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c26ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c26ea-114">Not supported.</span></span>|
|<span data-ttu-id="c26ea-115">Application</span><span class="sxs-lookup"><span data-stu-id="c26ea-115">Application</span></span>|<span data-ttu-id="c26ea-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ea-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c26ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c26ea-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c26ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c26ea-118">Optional query parameters</span></span>
<span data-ttu-id="c26ea-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c26ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ea-120">Request headers</span></span>
|<span data-ttu-id="c26ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c26ea-121">Header</span></span>        |<span data-ttu-id="c26ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c26ea-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="c26ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c26ea-123">Authorization</span></span> |<span data-ttu-id="c26ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c26ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c26ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c26ea-126">Content-Type</span></span>  |<span data-ttu-id="c26ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c26ea-127">application/json</span></span>         |
|<span data-ttu-id="c26ea-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="c26ea-128">If-Match</span></span>      |<span data-ttu-id="c26ea-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c26ea-129">Required.</span></span> <span data-ttu-id="c26ea-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos **diários,** os **diários** não serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="c26ea-130">When this request header is included and the eTag provided does not match the current tag on the **journals**, the **journals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c26ea-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ea-131">Request body</span></span>
<span data-ttu-id="c26ea-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c26ea-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="c26ea-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26ea-135">Response</span></span>
<span data-ttu-id="c26ea-136">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto diário **atualizado** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ea-136">If successful, this method returns a `200 OK` response code and an updated **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26ea-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c26ea-137">Example</span></span>

<span data-ttu-id="c26ea-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c26ea-138">**Request**</span></span>

<span data-ttu-id="c26ea-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c26ea-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}
Content-type: application/json

{
  "code": "EXPENSE",
  "displayName": "Expense Batch"
}
```

<span data-ttu-id="c26ea-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="c26ea-140">**Response**</span></span>

<span data-ttu-id="c26ea-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ea-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="c26ea-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c26ea-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "EXPENSE",
  "displayName": "Expense Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



