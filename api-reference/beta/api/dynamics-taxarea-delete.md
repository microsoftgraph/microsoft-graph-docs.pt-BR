---
title: Excluir taxAreas
description: Exclui um objeto de área de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3d50ae7f8e07a9338ba666e985d764e53a1f84c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008166"
---
# <a name="delete-taxareas"></a><span data-ttu-id="a5407-103">Excluir taxAreas</span><span class="sxs-lookup"><span data-stu-id="a5407-103">Delete taxAreas</span></span>

<span data-ttu-id="a5407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5407-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5407-105">Excluir um objeto de área de impostos do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a5407-105">Delete a tax area object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5407-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5407-106">Permissions</span></span>
<span data-ttu-id="a5407-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5407-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5407-109">Permission type</span></span> |<span data-ttu-id="a5407-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5407-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a5407-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5407-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5407-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5407-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a5407-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a5407-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a5407-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5407-114">Not supported.</span></span>|
|<span data-ttu-id="a5407-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5407-115">Application</span></span>|<span data-ttu-id="a5407-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5407-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5407-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5407-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5407-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5407-118">Optional query parameters</span></span>
<span data-ttu-id="a5407-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5407-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5407-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5407-120">Request headers</span></span>
|<span data-ttu-id="a5407-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5407-121">Header</span></span>|<span data-ttu-id="a5407-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a5407-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="a5407-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5407-123">Authorization</span></span>  |<span data-ttu-id="a5407-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5407-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a5407-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="a5407-126">If-Match</span></span>       |<span data-ttu-id="a5407-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5407-127">Required.</span></span> <span data-ttu-id="a5407-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **taxAreas**, o **taxAreas** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="a5407-128">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5407-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5407-129">Request body</span></span>

<span data-ttu-id="a5407-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5407-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5407-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5407-131">Response</span></span>

<span data-ttu-id="a5407-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5407-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5407-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5407-134">Example</span></span>

<span data-ttu-id="a5407-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a5407-135">**Request**</span></span>

<span data-ttu-id="a5407-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5407-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="a5407-137">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="a5407-137">**Response**</span></span> 

<span data-ttu-id="a5407-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5407-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```


