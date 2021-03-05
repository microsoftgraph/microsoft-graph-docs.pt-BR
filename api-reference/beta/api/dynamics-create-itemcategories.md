---
title: Criar itemCategories
description: Cria um objeto de categoria de item no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b50c1c9221c41c0e2bdb7cf5f24b4fbdd6ba9b13
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471352"
---
# <a name="create-itemcategories"></a><span data-ttu-id="3be3c-103">Criar itemCategories</span><span class="sxs-lookup"><span data-stu-id="3be3c-103">Create itemCategories</span></span>

<span data-ttu-id="3be3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be3c-105">Criar um objeto de categoria de item Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3be3c-105">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3be3c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3be3c-106">Permissions</span></span>
<span data-ttu-id="3be3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be3c-109">Permission type</span></span> |<span data-ttu-id="3be3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3be3c-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3be3c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3be3c-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be3c-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3be3c-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3be3c-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3be3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be3c-114">Not supported.</span></span>|
|<span data-ttu-id="3be3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be3c-115">Application</span></span>|<span data-ttu-id="3be3c-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be3c-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3be3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be3c-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3be3c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3be3c-118">Optional query parameters</span></span>
<span data-ttu-id="3be3c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3be3c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3be3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be3c-120">Request headers</span></span>
|<span data-ttu-id="3be3c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3be3c-121">Header</span></span>       |<span data-ttu-id="3be3c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3be3c-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="3be3c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be3c-123">Authorization</span></span>|<span data-ttu-id="3be3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be3c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3be3c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3be3c-126">Content-Type</span></span> |<span data-ttu-id="3be3c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3be3c-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="3be3c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be3c-128">Request body</span></span>
<span data-ttu-id="3be3c-129">No corpo da solicitação, fornece uma representação JSON de um **objeto itemCategories.**</span><span class="sxs-lookup"><span data-stu-id="3be3c-129">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="3be3c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be3c-130">Response</span></span>
<span data-ttu-id="3be3c-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **itemCategories** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be3c-131">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be3c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be3c-132">Example</span></span>

<span data-ttu-id="3be3c-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="3be3c-133">**Request**</span></span>

<span data-ttu-id="3be3c-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be3c-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="3be3c-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="3be3c-135">**Response**</span></span>

<span data-ttu-id="3be3c-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be3c-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="3be3c-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3be3c-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3be3c-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3be3c-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```






