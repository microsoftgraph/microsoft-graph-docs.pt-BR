---
title: Obter pagamentoMethods
description: Obtém um objeto de método de pagamento no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b2162578856b80deff2507ccf97222cb825f61a1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474313"
---
# <a name="get-paymentmethods"></a><span data-ttu-id="cfdee-103">Obter pagamentoMethods</span><span class="sxs-lookup"><span data-stu-id="cfdee-103">Get paymentMethods</span></span>

<span data-ttu-id="cfdee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfdee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfdee-105">Recupere as propriedades e as relações de um objeto de método de pagamento do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="cfdee-105">Retrieve the properties and relationships of a payment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfdee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfdee-106">Permissions</span></span>
<span data-ttu-id="cfdee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfdee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfdee-109">Permission type</span></span> |<span data-ttu-id="cfdee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfdee-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cfdee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfdee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cfdee-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdee-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cfdee-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cfdee-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cfdee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdee-114">Not supported.</span></span>|
|<span data-ttu-id="cfdee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfdee-115">Application</span></span>|<span data-ttu-id="cfdee-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdee-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfdee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdee-117">HTTP request</span></span>

```
GET /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfdee-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cfdee-118">Optional query parameters</span></span>
<span data-ttu-id="cfdee-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdee-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfdee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdee-120">Request headers</span></span>
|<span data-ttu-id="cfdee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfdee-121">Header</span></span>         |<span data-ttu-id="cfdee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfdee-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="cfdee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfdee-123">Authorization</span></span>  |<span data-ttu-id="cfdee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfdee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfdee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdee-126">Request body</span></span>
<span data-ttu-id="cfdee-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfdee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfdee-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdee-128">Response</span></span>
<span data-ttu-id="cfdee-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **paymentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdee-129">If successful, this method returns a `200 OK` response code and a **paymentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfdee-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfdee-130">Example</span></span>

<span data-ttu-id="cfdee-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="cfdee-131">**Request**</span></span>

<span data-ttu-id="cfdee-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfdee-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

<span data-ttu-id="cfdee-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="cfdee-133">**Response**</span></span>

<span data-ttu-id="cfdee-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdee-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="cfdee-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfdee-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cfdee-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfdee-136">All the properties will be returned from an actual call.</span></span>

```json
{

  "id": "id-value",
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```




