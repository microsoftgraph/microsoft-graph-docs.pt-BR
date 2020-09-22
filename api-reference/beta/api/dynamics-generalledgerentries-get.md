---
title: Obter generalLedgerEntries
description: Obtém um objeto de entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4aa22cf2a0634d9c54d6c9e12573730714be3ca4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981307"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="9271b-103">Obter generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="9271b-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="9271b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9271b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9271b-105">Recupere as propriedades e os relacionamentos de um objeto de entrada de contabilidade para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="9271b-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9271b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9271b-106">Permissions</span></span>
<span data-ttu-id="9271b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9271b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9271b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9271b-109">Permission type</span></span> |<span data-ttu-id="9271b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9271b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9271b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9271b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9271b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9271b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9271b-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9271b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9271b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9271b-114">Not supported.</span></span>|
|<span data-ttu-id="9271b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9271b-115">Application</span></span>|<span data-ttu-id="9271b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9271b-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="9271b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9271b-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9271b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9271b-118">Optional query parameters</span></span>
<span data-ttu-id="9271b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9271b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9271b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9271b-120">Request headers</span></span>
|<span data-ttu-id="9271b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9271b-121">Header</span></span>       |<span data-ttu-id="9271b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9271b-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="9271b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9271b-123">Authorization</span></span>|<span data-ttu-id="9271b-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="9271b-124">Bearer.</span></span> <span data-ttu-id="9271b-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9271b-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9271b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9271b-126">Request body</span></span>
<span data-ttu-id="9271b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9271b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9271b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9271b-128">Response</span></span>
<span data-ttu-id="9271b-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **generalLedgerEntries** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9271b-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9271b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9271b-130">Example</span></span>

<span data-ttu-id="9271b-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="9271b-131">**Request**</span></span>

<span data-ttu-id="9271b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9271b-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="9271b-133">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="9271b-133">**Response**</span></span>

<span data-ttu-id="9271b-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9271b-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="9271b-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9271b-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9271b-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9271b-136">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "10700",
    "postingDate": "2017-03-15",
    "documentNumber": "108027",
    "documentType": "Invoice",
    "accountId": "id-value",
    "accountNumber": "7210",
    "description": "Order 106003",
    "debitAmount": 6943.8,
    "creditAmount": 0,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```



