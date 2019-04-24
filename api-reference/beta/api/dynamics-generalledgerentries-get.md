---
title: Obter generalLedgerEntries
description: Obtém um objeto de entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 06884308987eb8010be965d30d09e064e3d67d5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458506"
---
# <a name="get-generalledgerentries"></a><span data-ttu-id="c61b8-103">Obter generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="c61b8-103">Get generalLedgerEntries</span></span>
<span data-ttu-id="c61b8-104">Recupere as propriedades e os relacionamentos de um objeto de entrada de contabilidade para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c61b8-104">Retrieve the properties and relationships of a general ledger entry object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c61b8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c61b8-105">Permissions</span></span>
<span data-ttu-id="c61b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c61b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61b8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c61b8-108">Permission type</span></span> |<span data-ttu-id="c61b8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c61b8-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c61b8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c61b8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c61b8-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61b8-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c61b8-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c61b8-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c61b8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c61b8-113">Not supported.</span></span>|
|<span data-ttu-id="c61b8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c61b8-114">Application</span></span>|<span data-ttu-id="c61b8-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61b8-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="c61b8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c61b8-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/generalLedgerEntries('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c61b8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c61b8-117">Optional query parameters</span></span>
<span data-ttu-id="c61b8-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c61b8-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c61b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c61b8-119">Request headers</span></span>
|<span data-ttu-id="c61b8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c61b8-120">Header</span></span>       |<span data-ttu-id="c61b8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c61b8-121">Value</span></span>             |
|-------------|------------------|
|<span data-ttu-id="c61b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c61b8-122">Authorization</span></span>|<span data-ttu-id="c61b8-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="c61b8-123">Bearer.</span></span> <span data-ttu-id="c61b8-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c61b8-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c61b8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c61b8-125">Request body</span></span>
<span data-ttu-id="c61b8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c61b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c61b8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c61b8-127">Response</span></span>
<span data-ttu-id="c61b8-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **generalLedgerEntries** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c61b8-128">If successful, this method returns a `200 OK` response code and a **generalLedgerEntries** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c61b8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c61b8-129">Example</span></span>

<span data-ttu-id="c61b8-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c61b8-130">**Request**</span></span>

<span data-ttu-id="c61b8-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c61b8-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/generalLedgerEntries('{id}')
```

<span data-ttu-id="c61b8-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="c61b8-132">**Response**</span></span>

<span data-ttu-id="c61b8-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c61b8-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="c61b8-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c61b8-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c61b8-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c61b8-135">All the properties will be returned from an actual call.</span></span>

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

