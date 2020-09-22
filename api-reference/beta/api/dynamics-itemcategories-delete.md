---
title: Excluir myCategories
description: Exclui uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f5739ea8e4109346c961c175804632c586db28b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981238"
---
# <a name="delete-itemcategories"></a><span data-ttu-id="2731a-103">Excluir myCategories</span><span class="sxs-lookup"><span data-stu-id="2731a-103">Delete itemCategories</span></span>

<span data-ttu-id="2731a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2731a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2731a-105">Exclua uma categoria do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2731a-105">Delete an itemCategory from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2731a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2731a-106">Permissions</span></span>
<span data-ttu-id="2731a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2731a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2731a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2731a-109">Permission type</span></span> |<span data-ttu-id="2731a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2731a-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2731a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2731a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2731a-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2731a-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2731a-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2731a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2731a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2731a-114">Not supported.</span></span>|
|<span data-ttu-id="2731a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2731a-115">Application</span></span>|<span data-ttu-id="2731a-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2731a-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2731a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2731a-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/itemCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2731a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2731a-118">Optional query parameters</span></span>
<span data-ttu-id="2731a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2731a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2731a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2731a-120">Request headers</span></span>
|<span data-ttu-id="2731a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2731a-121">Header</span></span>         |<span data-ttu-id="2731a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2731a-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="2731a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2731a-123">Authorization</span></span>  |<span data-ttu-id="2731a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2731a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="2731a-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="2731a-126">If-Match</span></span>       |<span data-ttu-id="2731a-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2731a-127">Required.</span></span> <span data-ttu-id="2731a-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **categorias**, as **categorias** não serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="2731a-128">When this request header is included and the eTag provided does not match the current tag on the **itemCategories**, the **itemCategories** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2731a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2731a-129">Request body</span></span>
<span data-ttu-id="2731a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2731a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2731a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2731a-131">Response</span></span>
<span data-ttu-id="2731a-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2731a-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2731a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2731a-134">Example</span></span>

<span data-ttu-id="2731a-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="2731a-135">**Request**</span></span>

<span data-ttu-id="2731a-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2731a-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories/{id}
```

<span data-ttu-id="2731a-137">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="2731a-137">**Response**</span></span> 

<span data-ttu-id="2731a-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2731a-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```



