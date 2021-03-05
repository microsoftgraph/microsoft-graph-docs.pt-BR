---
title: Obter shipmentMethods
description: Obtém um objeto de método de envio no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 92332f8ccec383738e77b7e0f613695411e2333c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474230"
---
# <a name="get-shipmentmethods"></a><span data-ttu-id="6890e-103">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="6890e-103">Get shipmentMethods</span></span>

<span data-ttu-id="6890e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6890e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6890e-105">Recupere as propriedades e as relações de um objeto de método de envio para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="6890e-105">Retrieve the properties and relationships of a shipment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6890e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6890e-106">Permissions</span></span>
<span data-ttu-id="6890e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6890e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6890e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6890e-109">Permission type</span></span> |<span data-ttu-id="6890e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6890e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6890e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6890e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6890e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6890e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6890e-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6890e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6890e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6890e-114">Not supported.</span></span>|
|<span data-ttu-id="6890e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6890e-115">Application</span></span>|<span data-ttu-id="6890e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6890e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6890e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6890e-117">HTTP request</span></span>

```
GET /financials/companies/{id}/shipmentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6890e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6890e-118">Optional query parameters</span></span>
<span data-ttu-id="6890e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6890e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6890e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6890e-120">Request headers</span></span>
|<span data-ttu-id="6890e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6890e-121">Header</span></span>|<span data-ttu-id="6890e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6890e-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="6890e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6890e-123">Authorization</span></span>  |<span data-ttu-id="6890e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6890e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6890e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6890e-126">Request body</span></span>
<span data-ttu-id="6890e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6890e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6890e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6890e-128">Response</span></span>
<span data-ttu-id="6890e-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **shipmentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6890e-129">If successful, this method returns a `200 OK` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6890e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6890e-130">Example</span></span>

<span data-ttu-id="6890e-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="6890e-131">**Request**</span></span>

<span data-ttu-id="6890e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6890e-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods/{id}
```

<span data-ttu-id="6890e-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="6890e-133">**Response**</span></span>

<span data-ttu-id="6890e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6890e-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="6890e-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6890e-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6890e-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6890e-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}
```



