---
title: Excluir moedas
description: Exclui um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 495800dbb9308971ef03172cc25602a15cffc103
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981538"
---
# <a name="delete-currencies"></a><span data-ttu-id="b1b34-103">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="b1b34-103">Delete currencies</span></span>

<span data-ttu-id="b1b34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b34-105">Excluir um objeto Currency do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b1b34-105">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1b34-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1b34-106">Permissions</span></span>
<span data-ttu-id="b1b34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1b34-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1b34-109">Permission type</span></span> |<span data-ttu-id="b1b34-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1b34-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b1b34-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1b34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1b34-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b34-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b1b34-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b1b34-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b1b34-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1b34-114">Not supported.</span></span>|
|<span data-ttu-id="b1b34-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1b34-115">Application</span></span>|<span data-ttu-id="b1b34-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b34-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1b34-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b34-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1b34-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1b34-118">Optional query parameters</span></span>
<span data-ttu-id="b1b34-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1b34-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1b34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1b34-120">Request headers</span></span>

|<span data-ttu-id="b1b34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1b34-121">Header</span></span>|<span data-ttu-id="b1b34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1b34-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="b1b34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1b34-123">Authorization</span></span>  |<span data-ttu-id="b1b34-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1b34-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b1b34-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="b1b34-126">If-Match</span></span>       |<span data-ttu-id="b1b34-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1b34-127">Required.</span></span> <span data-ttu-id="b1b34-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **moedas**, as **moedas** não serão</span><span class="sxs-lookup"><span data-stu-id="b1b34-128">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="b1b34-129">atualizado.</span><span class="sxs-lookup"><span data-stu-id="b1b34-129">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1b34-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1b34-130">Request body</span></span>
<span data-ttu-id="b1b34-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1b34-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1b34-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1b34-132">Response</span></span>
<span data-ttu-id="b1b34-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1b34-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b34-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1b34-135">Example</span></span>

<span data-ttu-id="b1b34-136">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b1b34-136">**Request**</span></span>

<span data-ttu-id="b1b34-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1b34-137">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="b1b34-138">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="b1b34-138">**Response**</span></span> 

<span data-ttu-id="b1b34-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1b34-139">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```


