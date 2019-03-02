---
title: Obter as categorias
description: Obtém uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7e339b89f53b0f7c3cd8f5dfc7976ba931bcaffd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365805"
---
# <a name="get-itemcategories"></a><span data-ttu-id="31f84-103">Obter as categorias</span><span class="sxs-lookup"><span data-stu-id="31f84-103">Get itemCategories</span></span>
<span data-ttu-id="31f84-104">Recupere as propriedades e os relacionamentos de um objeto de categoria de item para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="31f84-104">Retrieve the properties and relationships of an item category object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="31f84-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="31f84-105">Permissions</span></span>
<span data-ttu-id="31f84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31f84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31f84-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31f84-108">Permission type</span></span> |<span data-ttu-id="31f84-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31f84-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="31f84-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31f84-110">Delegated (work or school account)</span></span>|<span data-ttu-id="31f84-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f84-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="31f84-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="31f84-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="31f84-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31f84-113">Not supported.</span></span>|
|<span data-ttu-id="31f84-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31f84-114">Application</span></span>|<span data-ttu-id="31f84-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f84-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31f84-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31f84-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/itemCategories('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31f84-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31f84-117">Optional query parameters</span></span>
<span data-ttu-id="31f84-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="31f84-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31f84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31f84-119">Request headers</span></span>
|<span data-ttu-id="31f84-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31f84-120">Header</span></span>       |<span data-ttu-id="31f84-121">Valor</span><span class="sxs-lookup"><span data-stu-id="31f84-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="31f84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31f84-122">Authorization</span></span>|<span data-ttu-id="31f84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31f84-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31f84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31f84-125">Request body</span></span>
<span data-ttu-id="31f84-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31f84-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31f84-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="31f84-127">Response</span></span>
<span data-ttu-id="31f84-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto myCategories no corpo da resposta. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="31f84-128">If successful, this method returns a `200 OK` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31f84-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31f84-129">Example</span></span>

<span data-ttu-id="31f84-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="31f84-130">**Request**</span></span>

<span data-ttu-id="31f84-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31f84-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories('{id}')
```

<span data-ttu-id="31f84-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="31f84-132">**Response**</span></span>

<span data-ttu-id="31f84-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31f84-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="31f84-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31f84-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31f84-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31f84-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```

