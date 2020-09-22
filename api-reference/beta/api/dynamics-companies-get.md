---
title: Obter empresas
description: Obtém um objeto Company no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: cbf7abae89c7cc7c212920807b190b2072ef815d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008453"
---
# <a name="get-companies"></a><span data-ttu-id="863cc-103">Obter empresas</span><span class="sxs-lookup"><span data-stu-id="863cc-103">Get companies</span></span>

<span data-ttu-id="863cc-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="863cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863cc-105">Recupere as propriedades e os relacionamentos de um objeto de empresas para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="863cc-105">Retrieve the properties and relationships of a companies object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="863cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="863cc-106">Permissions</span></span>
<span data-ttu-id="863cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="863cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="863cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="863cc-109">Permission type</span></span> |<span data-ttu-id="863cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="863cc-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="863cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="863cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="863cc-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863cc-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="863cc-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="863cc-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="863cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="863cc-114">Not supported.</span></span>|
|<span data-ttu-id="863cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="863cc-115">Application</span></span>|<span data-ttu-id="863cc-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863cc-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="863cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="863cc-117">HTTP request</span></span>
```
GET /financials/companies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="863cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="863cc-118">Optional query parameters</span></span>
<span data-ttu-id="863cc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="863cc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="863cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="863cc-120">Request headers</span></span>
|<span data-ttu-id="863cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="863cc-121">Header</span></span>|<span data-ttu-id="863cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="863cc-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="863cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="863cc-123">Authorization</span></span>  |<span data-ttu-id="863cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="863cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="863cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="863cc-126">Request body</span></span>
<span data-ttu-id="863cc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="863cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="863cc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="863cc-128">Response</span></span>
<span data-ttu-id="863cc-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de **empresas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="863cc-129">If successful, this method returns a `200 OK` response code and a **companies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="863cc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="863cc-130">Example</span></span>

<span data-ttu-id="863cc-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="863cc-131">**Request**</span></span>

<span data-ttu-id="863cc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="863cc-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies
```

<span data-ttu-id="863cc-133">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="863cc-133">**Response**</span></span>

<span data-ttu-id="863cc-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="863cc-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="863cc-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="863cc-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="863cc-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="863cc-136">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "id-value",
    "systemVersion": "17806",
    "name": "CRONUS US",
    "displayName": "CRONUS USA, Inc.",
    "businessProfileId": ""
}
```


