---
title: Criar paymentMethods
description: Cria um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8c6512c6539dbc48fb3d35124370ec672a4759ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431341"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="65970-103">Criar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="65970-103">Create paymentMethods</span></span>

<span data-ttu-id="65970-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65970-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65970-105">Criar um objeto de método de pagamento no DDynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="65970-105">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="65970-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65970-106">Permissions</span></span>
<span data-ttu-id="65970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65970-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65970-109">Permission type</span></span> |<span data-ttu-id="65970-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65970-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="65970-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65970-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65970-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65970-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="65970-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="65970-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="65970-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65970-114">Not supported.</span></span>|
|<span data-ttu-id="65970-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65970-115">Application</span></span>|<span data-ttu-id="65970-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65970-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65970-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65970-117">HTTP request</span></span>
```
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65970-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65970-118">Optional query parameters</span></span>
<span data-ttu-id="65970-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65970-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65970-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65970-120">Request headers</span></span>
|<span data-ttu-id="65970-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65970-121">Header</span></span>         |<span data-ttu-id="65970-122">Valor</span><span class="sxs-lookup"><span data-stu-id="65970-122">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="65970-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="65970-123">Authorization</span></span>  |<span data-ttu-id="65970-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65970-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="65970-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65970-126">Content-Type</span></span>   |<span data-ttu-id="65970-127">application/json</span><span class="sxs-lookup"><span data-stu-id="65970-127">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="65970-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65970-128">Request body</span></span>
<span data-ttu-id="65970-129">No corpo da solicitação, forneça uma representação JSON de um objeto **paymentMethods** .</span><span class="sxs-lookup"><span data-stu-id="65970-129">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="65970-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="65970-130">Response</span></span>
<span data-ttu-id="65970-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **paymentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65970-131">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65970-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65970-132">Example</span></span>

<span data-ttu-id="65970-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="65970-133">**Request**</span></span>

<span data-ttu-id="65970-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="65970-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="65970-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="65970-135">**Response**</span></span>

<span data-ttu-id="65970-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65970-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="65970-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65970-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65970-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65970-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```

