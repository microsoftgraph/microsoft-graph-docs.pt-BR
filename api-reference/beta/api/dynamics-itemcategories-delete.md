---
title: Excluir myCategories
description: Exclui uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f422685568c08590a0ba7c8cc7a5fe578f50d9a6
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791558"
---
# <a name="delete-itemcategories"></a><span data-ttu-id="dc2fe-103">Excluir myCategories</span><span class="sxs-lookup"><span data-stu-id="dc2fe-103">Delete itemCategories</span></span>
<span data-ttu-id="dc2fe-104">Exclua uma categoria do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-104">Delete an itemCategory from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc2fe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc2fe-105">Permissions</span></span>
<span data-ttu-id="dc2fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2fe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc2fe-108">Permission type</span></span> |<span data-ttu-id="dc2fe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc2fe-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="dc2fe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc2fe-110">Delegated (work or school account)</span></span>|<span data-ttu-id="dc2fe-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2fe-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="dc2fe-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="dc2fe-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="dc2fe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-113">Not supported.</span></span>|
|<span data-ttu-id="dc2fe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc2fe-114">Application</span></span>|<span data-ttu-id="dc2fe-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2fe-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc2fe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc2fe-116">HTTP request</span></span>
```
DELETE /financials/companies/{id}/itemCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc2fe-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc2fe-117">Optional query parameters</span></span>
<span data-ttu-id="dc2fe-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc2fe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2fe-119">Request headers</span></span>
|<span data-ttu-id="dc2fe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc2fe-120">Header</span></span>         |<span data-ttu-id="dc2fe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc2fe-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="dc2fe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc2fe-122">Authorization</span></span>  |<span data-ttu-id="dc2fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="dc2fe-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="dc2fe-125">If-Match</span></span>       |<span data-ttu-id="dc2fe-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-126">Required.</span></span> <span data-ttu-id="dc2fe-127">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **categorias**, as **categorias** não serão atualizadas.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-127">When this request header is included and the eTag provided does not match the current tag on the **itemCategories**, the **itemCategories** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc2fe-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2fe-128">Request body</span></span>
<span data-ttu-id="dc2fe-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc2fe-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc2fe-130">Response</span></span>
<span data-ttu-id="dc2fe-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc2fe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc2fe-133">Example</span></span>

<span data-ttu-id="dc2fe-134">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="dc2fe-134">**Request**</span></span>

<span data-ttu-id="dc2fe-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories/{id}
```

<span data-ttu-id="dc2fe-136">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="dc2fe-136">**Response**</span></span> 

<span data-ttu-id="dc2fe-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2fe-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

