---
title: Atualizar taxAreas
description: Atualiza um objeto de áreas fiscais no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a2f8a3321b1143d367ce4c256e97cf42af77b100
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474164"
---
# <a name="update-taxareas"></a><span data-ttu-id="4af5c-103">Atualizar taxAreas</span><span class="sxs-lookup"><span data-stu-id="4af5c-103">Update taxAreas</span></span>

<span data-ttu-id="4af5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4af5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4af5c-105">Atualize as propriedades de um objeto de área fiscal para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="4af5c-105">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4af5c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4af5c-106">Permissions</span></span>
<span data-ttu-id="4af5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4af5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4af5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4af5c-109">Permission type</span></span> |<span data-ttu-id="4af5c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4af5c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4af5c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4af5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4af5c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4af5c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4af5c-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4af5c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4af5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af5c-114">Not supported.</span></span>|
|<span data-ttu-id="4af5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4af5c-115">Application</span></span>|<span data-ttu-id="4af5c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4af5c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4af5c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4af5c-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4af5c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4af5c-118">Optional query parameters</span></span>
<span data-ttu-id="4af5c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4af5c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4af5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4af5c-120">Request headers</span></span>
|<span data-ttu-id="4af5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4af5c-121">Header</span></span>|<span data-ttu-id="4af5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4af5c-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="4af5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4af5c-123">Authorization</span></span> |<span data-ttu-id="4af5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4af5c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4af5c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4af5c-126">Content-Type</span></span>  |<span data-ttu-id="4af5c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4af5c-127">application/json</span></span>|
|<span data-ttu-id="4af5c-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="4af5c-128">If-Match</span></span>      |<span data-ttu-id="4af5c-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4af5c-129">Required.</span></span> <span data-ttu-id="4af5c-130">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **taxAreas**, **o taxAreas** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="4af5c-130">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4af5c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4af5c-131">Request body</span></span>
<span data-ttu-id="4af5c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4af5c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4af5c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af5c-135">Response</span></span>
<span data-ttu-id="4af5c-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **objeto taxAreas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4af5c-136">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4af5c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4af5c-137">Example</span></span>

<span data-ttu-id="4af5c-138">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4af5c-138">**Request**</span></span>

<span data-ttu-id="4af5c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4af5c-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="4af5c-140">**Response**</span><span class="sxs-lookup"><span data-stu-id="4af5c-140">**Response**</span></span>

<span data-ttu-id="4af5c-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4af5c-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="4af5c-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4af5c-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4af5c-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4af5c-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



