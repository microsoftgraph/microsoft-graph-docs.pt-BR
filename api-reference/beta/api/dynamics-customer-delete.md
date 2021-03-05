---
title: Excluir clientes
description: Exclui um objeto customers do Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: de4976e6a80fd54db75fc0e4111c7fa22746f535
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471329"
---
# <a name="delete-customers"></a><span data-ttu-id="721df-103">Excluir clientes</span><span class="sxs-lookup"><span data-stu-id="721df-103">Delete customers</span></span>

<span data-ttu-id="721df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="721df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="721df-105">Exclua um objeto do cliente do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="721df-105">Delete a customer object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="721df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="721df-106">Permissions</span></span>
<span data-ttu-id="721df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="721df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="721df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="721df-109">Permission type</span></span> |<span data-ttu-id="721df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="721df-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="721df-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="721df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="721df-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721df-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="721df-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="721df-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="721df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="721df-114">Not supported.</span></span>|
|<span data-ttu-id="721df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="721df-115">Application</span></span>|<span data-ttu-id="721df-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721df-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="721df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="721df-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="721df-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="721df-118">Optional query parameters</span></span>
<span data-ttu-id="721df-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="721df-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="721df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="721df-120">Request headers</span></span>
|<span data-ttu-id="721df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="721df-121">Header</span></span>         |<span data-ttu-id="721df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="721df-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="721df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="721df-123">Authorization</span></span>  |<span data-ttu-id="721df-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="721df-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="721df-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="721df-126">If-Match</span></span>       |<span data-ttu-id="721df-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="721df-127">Required.</span></span> <span data-ttu-id="721df-128">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos clientes **,** os clientes **não** serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="721df-128">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="721df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="721df-129">Request body</span></span>
<span data-ttu-id="721df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="721df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="721df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="721df-131">Response</span></span>
<span data-ttu-id="721df-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="721df-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="721df-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="721df-134">Example</span></span>

<span data-ttu-id="721df-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="721df-135">**Request**</span></span>

<span data-ttu-id="721df-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="721df-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="721df-137">**Response**</span><span class="sxs-lookup"><span data-stu-id="721df-137">**Response**</span></span> 

<span data-ttu-id="721df-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="721df-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```



