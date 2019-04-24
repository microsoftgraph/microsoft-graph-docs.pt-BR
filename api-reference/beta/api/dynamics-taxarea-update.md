---
title: Atualizar taxAreas
description: Atualiza um objeto de áreas de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42a53f03e71ca5fe41293db0dc5459990f4560e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458296"
---
# <a name="update-taxareas"></a><span data-ttu-id="3b489-103">Atualizar taxAreas</span><span class="sxs-lookup"><span data-stu-id="3b489-103">Update taxAreas</span></span>
<span data-ttu-id="3b489-104">Atualizar as propriedades de um objeto de área de impostos para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3b489-104">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b489-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b489-105">Permissions</span></span>
<span data-ttu-id="3b489-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b489-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b489-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b489-108">Permission type</span></span> |<span data-ttu-id="3b489-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b489-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3b489-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b489-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3b489-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b489-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3b489-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3b489-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3b489-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b489-113">Not supported.</span></span>|
|<span data-ttu-id="3b489-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b489-114">Application</span></span>|<span data-ttu-id="3b489-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b489-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b489-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b489-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b489-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b489-117">Optional query parameters</span></span>
<span data-ttu-id="3b489-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3b489-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b489-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b489-119">Request headers</span></span>
|<span data-ttu-id="3b489-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b489-120">Header</span></span>|<span data-ttu-id="3b489-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b489-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3b489-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b489-122">Authorization</span></span> |<span data-ttu-id="3b489-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b489-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3b489-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b489-125">Content-Type</span></span>  |<span data-ttu-id="3b489-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b489-126">application/json</span></span>|
|<span data-ttu-id="3b489-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="3b489-127">If-Match</span></span>      |<span data-ttu-id="3b489-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b489-128">Required.</span></span> <span data-ttu-id="3b489-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **taxAreas**, o **taxAreas** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="3b489-129">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b489-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b489-130">Request body</span></span>
<span data-ttu-id="3b489-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3b489-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="3b489-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b489-134">Response</span></span>
<span data-ttu-id="3b489-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **taxAreas** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b489-135">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b489-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b489-136">Example</span></span>

<span data-ttu-id="3b489-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="3b489-137">**Request**</span></span>

<span data-ttu-id="3b489-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b489-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas('{id}')
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="3b489-139">**Response**</span><span class="sxs-lookup"><span data-stu-id="3b489-139">**Response**</span></span>

<span data-ttu-id="3b489-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b489-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="3b489-141">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3b489-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3b489-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b489-142">All the properties will be returned from an actual call.</span></span>

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

