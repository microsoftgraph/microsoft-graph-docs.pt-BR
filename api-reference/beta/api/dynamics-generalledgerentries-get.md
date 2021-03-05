---
title: Obter generalLedgerEntries
description: Obtém um objeto de entrada de livro-razão geral no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d3862417cd75e2a6adb55c1c9660b8b1c2ddabc4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473004"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="48998-103">Obter generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="48998-103">Get generalLedgerEntries</span></span>

<span data-ttu-id="48998-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48998-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48998-105">Recupere as propriedades e as relações de um objeto de entrada de livro-razão geral para o Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="48998-105">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="48998-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="48998-106">Permissions</span></span>
<span data-ttu-id="48998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48998-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48998-109">Permission type</span></span> |<span data-ttu-id="48998-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48998-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="48998-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48998-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48998-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48998-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="48998-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="48998-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="48998-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48998-114">Not supported.</span></span>|
|<span data-ttu-id="48998-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48998-115">Application</span></span>|<span data-ttu-id="48998-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48998-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="48998-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48998-117">HTTP request</span></span>
```
GET /financials/companies/{id}/generalLedgerEntries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48998-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="48998-118">Optional query parameters</span></span>
<span data-ttu-id="48998-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48998-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48998-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48998-120">Request headers</span></span>
|<span data-ttu-id="48998-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48998-121">Header</span></span>       |<span data-ttu-id="48998-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48998-122">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="48998-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48998-123">Authorization</span></span>|<span data-ttu-id="48998-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="48998-124">Bearer.</span></span> <span data-ttu-id="48998-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48998-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48998-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48998-126">Request body</span></span>
<span data-ttu-id="48998-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48998-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48998-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="48998-128">Response</span></span>
<span data-ttu-id="48998-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **objeto generalLedgerEntries** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48998-129">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48998-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48998-130">Example</span></span>

<span data-ttu-id="48998-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="48998-131">**Request**</span></span>

<span data-ttu-id="48998-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48998-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/generalLedgerEntries/{id}
```

<span data-ttu-id="48998-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="48998-133">**Response**</span></span>

<span data-ttu-id="48998-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48998-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="48998-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48998-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48998-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48998-136">All the properties will be returned from an actual call.</span></span>

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



