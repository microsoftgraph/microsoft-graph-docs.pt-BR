---
title: Excluir moedas
description: Exclui um objeto currency no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b9f6c729dc97d523952454978afc056c05c354c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473151"
---
# <a name="delete-currencies"></a><span data-ttu-id="a9608-103">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="a9608-103">Delete currencies</span></span>

<span data-ttu-id="a9608-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9608-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9608-105">Exclua um objeto currency do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a9608-105">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9608-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9608-106">Permissions</span></span>
<span data-ttu-id="a9608-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9608-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9608-109">Permission type</span></span> |<span data-ttu-id="a9608-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9608-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a9608-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9608-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9608-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9608-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a9608-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a9608-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a9608-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9608-114">Not supported.</span></span>|
|<span data-ttu-id="a9608-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9608-115">Application</span></span>|<span data-ttu-id="a9608-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9608-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9608-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9608-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9608-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9608-118">Optional query parameters</span></span>
<span data-ttu-id="a9608-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9608-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9608-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9608-120">Request headers</span></span>

|<span data-ttu-id="a9608-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9608-121">Header</span></span>|<span data-ttu-id="a9608-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9608-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a9608-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9608-123">Authorization</span></span>  |<span data-ttu-id="a9608-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9608-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a9608-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="a9608-126">If-Match</span></span>       |<span data-ttu-id="a9608-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9608-127">Required.</span></span> <span data-ttu-id="a9608-128">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas moedas **,** as moedas **não** serão</span><span class="sxs-lookup"><span data-stu-id="a9608-128">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="a9608-129">atualizado.</span><span class="sxs-lookup"><span data-stu-id="a9608-129">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9608-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9608-130">Request body</span></span>
<span data-ttu-id="a9608-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9608-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9608-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9608-132">Response</span></span>
<span data-ttu-id="a9608-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9608-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9608-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9608-135">Example</span></span>

<span data-ttu-id="a9608-136">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a9608-136">**Request**</span></span>

<span data-ttu-id="a9608-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9608-137">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="a9608-138">**Response**</span><span class="sxs-lookup"><span data-stu-id="a9608-138">**Response**</span></span> 

<span data-ttu-id="a9608-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9608-139">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```


