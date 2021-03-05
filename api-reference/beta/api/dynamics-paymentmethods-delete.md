---
title: Excluir paymentMethods
description: Exclui um objeto de método de pagamento no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f02b2c82386180609afbf13beeb25b35c6a30467
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474320"
---
# <a name="delete-paymentmethods"></a><span data-ttu-id="77c38-103">Excluir paymentMethods</span><span class="sxs-lookup"><span data-stu-id="77c38-103">Delete paymentMethods</span></span>

<span data-ttu-id="77c38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c38-105">Exclua um objeto de método de pagamento do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="77c38-105">Delete a payment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="77c38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77c38-106">Permissions</span></span>
<span data-ttu-id="77c38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77c38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77c38-109">Permission type</span></span> |<span data-ttu-id="77c38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77c38-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="77c38-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77c38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77c38-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c38-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="77c38-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="77c38-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="77c38-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77c38-114">Not supported.</span></span>|
|<span data-ttu-id="77c38-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77c38-115">Application</span></span>|<span data-ttu-id="77c38-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c38-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77c38-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77c38-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77c38-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77c38-118">Optional query parameters</span></span>
<span data-ttu-id="77c38-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77c38-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77c38-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77c38-120">Request headers</span></span>

|<span data-ttu-id="77c38-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77c38-121">Header</span></span>         |<span data-ttu-id="77c38-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77c38-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="77c38-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77c38-123">Authorization</span></span>  |<span data-ttu-id="77c38-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77c38-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="77c38-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="77c38-126">If-Match</span></span>       |<span data-ttu-id="77c38-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77c38-127">Required.</span></span> <span data-ttu-id="77c38-128">Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **pagamentoMethods,** o **pagamentoMethods** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="77c38-128">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77c38-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77c38-129">Request body</span></span>
<span data-ttu-id="77c38-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77c38-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77c38-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="77c38-131">Response</span></span>
<span data-ttu-id="77c38-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77c38-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77c38-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77c38-134">Example</span></span>

<span data-ttu-id="77c38-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="77c38-135">**Request**</span></span>

<span data-ttu-id="77c38-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77c38-136">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

<span data-ttu-id="77c38-137">**Response**</span><span class="sxs-lookup"><span data-stu-id="77c38-137">**Response**</span></span> 

<span data-ttu-id="77c38-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77c38-138">Here is an example of the response.</span></span> 

```http
HTTP/1.1 204 No Content
```



