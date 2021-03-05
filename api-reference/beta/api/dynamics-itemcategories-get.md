---
title: Obter itemCategories
description: Obtém uma categoria de item no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6e74210fc5f2a4e8b4d91f93a9df3b57d2a35962
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472913"
---
# <a name="get-itemcategories"></a><span data-ttu-id="51822-103">Obter itemCategories</span><span class="sxs-lookup"><span data-stu-id="51822-103">Get itemCategories</span></span>

<span data-ttu-id="51822-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51822-105">Recupere as propriedades e as relações de um objeto de categoria de item para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="51822-105">Retrieve the properties and relationships of an item category object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="51822-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="51822-106">Permissions</span></span>
<span data-ttu-id="51822-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51822-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51822-109">Permission type</span></span> |<span data-ttu-id="51822-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51822-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="51822-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51822-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51822-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51822-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="51822-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="51822-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="51822-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51822-114">Not supported.</span></span>|
|<span data-ttu-id="51822-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51822-115">Application</span></span>|<span data-ttu-id="51822-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51822-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51822-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51822-117">HTTP request</span></span>

```
GET /financials/companies/{id}/itemCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51822-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51822-118">Optional query parameters</span></span>
<span data-ttu-id="51822-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51822-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51822-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51822-120">Request headers</span></span>
|<span data-ttu-id="51822-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51822-121">Header</span></span>       |<span data-ttu-id="51822-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51822-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="51822-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51822-123">Authorization</span></span>|<span data-ttu-id="51822-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51822-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51822-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51822-126">Request body</span></span>
<span data-ttu-id="51822-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51822-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51822-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="51822-128">Response</span></span>
<span data-ttu-id="51822-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **itemCategories** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51822-129">If successful, this method returns a `200 OK` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51822-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51822-130">Example</span></span>

<span data-ttu-id="51822-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="51822-131">**Request**</span></span>

<span data-ttu-id="51822-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51822-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories/{id}
```

<span data-ttu-id="51822-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="51822-133">**Response**</span></span>

<span data-ttu-id="51822-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51822-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="51822-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51822-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51822-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51822-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```



