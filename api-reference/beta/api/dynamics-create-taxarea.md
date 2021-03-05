---
title: Criar taxAreas
description: Cria um objeto de área fiscal no Dynamics for Financials.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e30275efd4205b776593b5d515b2032654506a90
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473235"
---
# <a name="create-taxareas"></a><span data-ttu-id="bfe4c-103">Criar taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfe4c-103">Create taxAreas</span></span>

<span data-ttu-id="bfe4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe4c-105">Cria um objeto de área fiscal no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfe4c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfe4c-106">Permissions</span></span>
<span data-ttu-id="bfe4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfe4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe4c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfe4c-109">Permission type</span></span> |<span data-ttu-id="bfe4c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfe4c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bfe4c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfe4c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfe4c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfe4c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bfe4c-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bfe4c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bfe4c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-114">Not supported.</span></span>|
|<span data-ttu-id="bfe4c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfe4c-115">Application</span></span>|<span data-ttu-id="bfe4c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfe4c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfe4c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfe4c-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfe4c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfe4c-118">Optional query parameters</span></span>
<span data-ttu-id="bfe4c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfe4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfe4c-120">Request headers</span></span>
|<span data-ttu-id="bfe4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bfe4c-121">Header</span></span>|<span data-ttu-id="bfe4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bfe4c-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="bfe4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfe4c-123">Authorization</span></span>  |<span data-ttu-id="bfe4c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="bfe4c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfe4c-126">Content-Type</span></span>  |<span data-ttu-id="bfe4c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bfe4c-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="bfe4c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfe4c-128">Request body</span></span>
<span data-ttu-id="bfe4c-129">No corpo da solicitação, fornece uma representação JSON de um **objeto taxAreas.**</span><span class="sxs-lookup"><span data-stu-id="bfe4c-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="bfe4c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfe4c-130">Response</span></span>
<span data-ttu-id="bfe4c-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **taxAreas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfe4c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfe4c-132">Example</span></span>

<span data-ttu-id="bfe4c-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="bfe4c-133">**Request**</span></span>

<span data-ttu-id="bfe4c-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfe4c-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

{
  "code": "44442001T"
}
```

<span data-ttu-id="bfe4c-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="bfe4c-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


