---
title: Criar paymentMethods
description: Cria um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 08ef2450c06040820dac0b1807c16382bff262dd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366743"
---
# <a name="create-paymentmethods"></a><span data-ttu-id="a3bb0-103">Criar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="a3bb0-103">Create paymentMethods</span></span>
<span data-ttu-id="a3bb0-104">Criar um objeto de método de pagamento no DDynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-104">Create a payment method object in DDynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3bb0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3bb0-105">Permissions</span></span>
<span data-ttu-id="a3bb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bb0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3bb0-108">Permission type</span></span> |<span data-ttu-id="a3bb0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3bb0-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a3bb0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3bb0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a3bb0-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bb0-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a3bb0-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a3bb0-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a3bb0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-113">Not supported.</span></span>|
|<span data-ttu-id="a3bb0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3bb0-114">Application</span></span>|<span data-ttu-id="a3bb0-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bb0-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3bb0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3bb0-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/paymentMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3bb0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3bb0-117">Optional query parameters</span></span>
<span data-ttu-id="a3bb0-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3bb0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3bb0-119">Request headers</span></span>
|<span data-ttu-id="a3bb0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3bb0-120">Header</span></span>         |<span data-ttu-id="a3bb0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a3bb0-121">Value</span></span>                        |
|---------------|-----------------------------|
|<span data-ttu-id="a3bb0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3bb0-122">Authorization</span></span>  |<span data-ttu-id="a3bb0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="a3bb0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3bb0-125">Content-Type</span></span>   |<span data-ttu-id="a3bb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bb0-126">application/json</span></span>             |

## <a name="request-body"></a><span data-ttu-id="a3bb0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3bb0-127">Request body</span></span>
<span data-ttu-id="a3bb0-128">No corpo da solicitação, forneça uma representação JSON de um objeto **paymentMethods** .</span><span class="sxs-lookup"><span data-stu-id="a3bb0-128">In the request body, supply a JSON representation of a **paymentMethods** object.</span></span>

## <a name="response"></a><span data-ttu-id="a3bb0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3bb0-129">Response</span></span>
<span data-ttu-id="a3bb0-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **paymentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-130">If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bb0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3bb0-131">Example</span></span>

<span data-ttu-id="a3bb0-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a3bb0-132">**Request**</span></span>

<span data-ttu-id="a3bb0-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
}
```

<span data-ttu-id="a3bb0-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="a3bb0-134">**Response**</span></span>

<span data-ttu-id="a3bb0-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="a3bb0-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a3bb0-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3bb0-137">All the properties will be returned from an actual call.</span></span>

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

