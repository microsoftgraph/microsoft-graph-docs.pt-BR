---
title: Excluir fornecedores
description: Exclui um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: daafbc248d79fe5189060d4b52388c7715f29086
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427932"
---
# <a name="delete-vendors"></a><span data-ttu-id="68503-103">Excluir fornecedores</span><span class="sxs-lookup"><span data-stu-id="68503-103">Delete vendors</span></span>

<span data-ttu-id="68503-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68503-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68503-105">Excluir um objeto fornecedor do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="68503-105">Delete a vendor object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="68503-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68503-106">Permissions</span></span>
<span data-ttu-id="68503-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68503-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68503-109">Permission type</span></span> |<span data-ttu-id="68503-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68503-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="68503-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68503-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68503-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68503-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="68503-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="68503-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="68503-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68503-114">Not supported.</span></span>|
|<span data-ttu-id="68503-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68503-115">Application</span></span>|<span data-ttu-id="68503-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68503-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68503-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68503-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68503-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68503-118">Optional query parameters</span></span>
<span data-ttu-id="68503-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68503-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68503-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68503-120">Request headers</span></span>
|<span data-ttu-id="68503-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68503-121">Header</span></span>|<span data-ttu-id="68503-122">Valor</span><span class="sxs-lookup"><span data-stu-id="68503-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="68503-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="68503-123">Authorization</span></span>  |<span data-ttu-id="68503-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68503-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="68503-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="68503-126">If-Match</span></span>       |<span data-ttu-id="68503-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68503-127">Required.</span></span> <span data-ttu-id="68503-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos **fornecedores**, os **fornecedores** não serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="68503-128">When this request header is included and the eTag provided does not match the current tag on the **vendors**, the **vendors** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68503-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68503-129">Request body</span></span>
<span data-ttu-id="68503-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68503-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68503-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="68503-131">Response</span></span>
<span data-ttu-id="68503-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68503-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68503-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68503-134">Example</span></span>

<span data-ttu-id="68503-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="68503-135">**Request**</span></span>

<span data-ttu-id="68503-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68503-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="68503-137">**Response**</span><span class="sxs-lookup"><span data-stu-id="68503-137">**Response**</span></span> 

<span data-ttu-id="68503-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68503-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
