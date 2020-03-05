---
title: Excluir moedas
description: Exclui um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8900330ed7f7f62aa9f2ba3de05aef01044cbbeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431040"
---
# <a name="delete-currencies"></a><span data-ttu-id="35d3d-103">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="35d3d-103">Delete currencies</span></span>

<span data-ttu-id="35d3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35d3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35d3d-105">Excluir um objeto Currency do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="35d3d-105">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="35d3d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35d3d-106">Permissions</span></span>
<span data-ttu-id="35d3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35d3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35d3d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35d3d-109">Permission type</span></span> |<span data-ttu-id="35d3d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35d3d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="35d3d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35d3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35d3d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35d3d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="35d3d-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="35d3d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="35d3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35d3d-114">Not supported.</span></span>|
|<span data-ttu-id="35d3d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35d3d-115">Application</span></span>|<span data-ttu-id="35d3d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35d3d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35d3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35d3d-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35d3d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="35d3d-118">Optional query parameters</span></span>
<span data-ttu-id="35d3d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="35d3d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35d3d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35d3d-120">Request headers</span></span>

|<span data-ttu-id="35d3d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35d3d-121">Header</span></span>|<span data-ttu-id="35d3d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35d3d-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="35d3d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35d3d-123">Authorization</span></span>  |<span data-ttu-id="35d3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35d3d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="35d3d-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="35d3d-126">If-Match</span></span>       |<span data-ttu-id="35d3d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35d3d-127">Required.</span></span> <span data-ttu-id="35d3d-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **moedas**, as **moedas** não serão</span><span class="sxs-lookup"><span data-stu-id="35d3d-128">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="35d3d-129">atualizado.</span><span class="sxs-lookup"><span data-stu-id="35d3d-129">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35d3d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35d3d-130">Request body</span></span>
<span data-ttu-id="35d3d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35d3d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35d3d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="35d3d-132">Response</span></span>
<span data-ttu-id="35d3d-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35d3d-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35d3d-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35d3d-135">Example</span></span>

<span data-ttu-id="35d3d-136">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="35d3d-136">**Request**</span></span>

<span data-ttu-id="35d3d-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35d3d-137">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="35d3d-138">**Response**</span><span class="sxs-lookup"><span data-stu-id="35d3d-138">**Response**</span></span> 

<span data-ttu-id="35d3d-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35d3d-139">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
