---
title: Criar paymentMethods
description: Cria um objeto de método de pagamento no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 64d7dac3590845f4fa4a95de9fc32829654a1d57
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473272"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="ef99f-103">Criar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="ef99f-103">Create paymentMethods</span></span>

<span data-ttu-id="ef99f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef99f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef99f-105">Crie um objeto de método de pagamento no DDynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ef99f-105">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef99f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef99f-106">Permissions</span></span>
<span data-ttu-id="ef99f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef99f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef99f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef99f-109">Permission type</span></span> |<span data-ttu-id="ef99f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef99f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ef99f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef99f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef99f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef99f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ef99f-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ef99f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ef99f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef99f-114">Not supported.</span></span>|
|<span data-ttu-id="ef99f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef99f-115">Application</span></span>|<span data-ttu-id="ef99f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef99f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef99f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef99f-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef99f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ef99f-118">Optional query parameters</span></span>
<span data-ttu-id="ef99f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ef99f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef99f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef99f-120">Request headers</span></span>
|<span data-ttu-id="ef99f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef99f-121">Header</span></span>         |<span data-ttu-id="ef99f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef99f-122">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="ef99f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef99f-123">Authorization</span></span>  |<span data-ttu-id="ef99f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef99f-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="ef99f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef99f-126">Content-Type</span></span>   |<span data-ttu-id="ef99f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ef99f-127">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="ef99f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef99f-128">Request body</span></span>
<span data-ttu-id="ef99f-129">No corpo da solicitação, fornece uma representação JSON de um **objeto paymentMethods.**</span><span class="sxs-lookup"><span data-stu-id="ef99f-129">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="ef99f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef99f-130">Response</span></span>
<span data-ttu-id="ef99f-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **paymentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef99f-131">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef99f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef99f-132">Example</span></span>

<span data-ttu-id="ef99f-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="ef99f-133">**Request**</span></span>

<span data-ttu-id="ef99f-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef99f-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="ef99f-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="ef99f-135">**Response**</span></span>

<span data-ttu-id="ef99f-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef99f-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="ef99f-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef99f-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef99f-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef99f-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```



