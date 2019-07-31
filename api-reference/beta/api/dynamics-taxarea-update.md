---
title: Atualizar taxAreas
description: Atualiza um objeto de áreas de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c6c3cedd16e8cca7a801d597718482ef1b6c12a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955922"
---
# <a name="update-taxareas"></a><span data-ttu-id="6d5d7-103">Atualizar taxAreas</span><span class="sxs-lookup"><span data-stu-id="6d5d7-103">Update taxAreas</span></span>
<span data-ttu-id="6d5d7-104">Atualizar as propriedades de um objeto de área de impostos para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-104">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d5d7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d5d7-105">Permissions</span></span>
<span data-ttu-id="6d5d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d5d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d5d7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d5d7-108">Permission type</span></span> |<span data-ttu-id="6d5d7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d5d7-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6d5d7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d5d7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6d5d7-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d5d7-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6d5d7-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6d5d7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6d5d7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-113">Not supported.</span></span>|
|<span data-ttu-id="6d5d7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d5d7-114">Application</span></span>|<span data-ttu-id="6d5d7-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d5d7-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d5d7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d5d7-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d5d7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d5d7-117">Optional query parameters</span></span>
<span data-ttu-id="6d5d7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d5d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d5d7-119">Request headers</span></span>
|<span data-ttu-id="6d5d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d5d7-120">Header</span></span>|<span data-ttu-id="6d5d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d5d7-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="6d5d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d5d7-122">Authorization</span></span> |<span data-ttu-id="6d5d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6d5d7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d5d7-125">Content-Type</span></span>  |<span data-ttu-id="6d5d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d5d7-126">application/json</span></span>|
|<span data-ttu-id="6d5d7-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="6d5d7-127">If-Match</span></span>      |<span data-ttu-id="6d5d7-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-128">Required.</span></span> <span data-ttu-id="6d5d7-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **taxAreas**, o **taxAreas** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-129">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d5d7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d5d7-130">Request body</span></span>
<span data-ttu-id="6d5d7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="6d5d7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d5d7-134">Response</span></span>
<span data-ttu-id="6d5d7-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **taxAreas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-135">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d5d7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d5d7-136">Example</span></span>

<span data-ttu-id="6d5d7-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="6d5d7-137">**Request**</span></span>

<span data-ttu-id="6d5d7-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas('{id}')
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="6d5d7-139">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="6d5d7-139">**Response**</span></span>

<span data-ttu-id="6d5d7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="6d5d7-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d5d7-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d5d7-142">All the properties will be returned from an actual call.</span></span>

```json
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

