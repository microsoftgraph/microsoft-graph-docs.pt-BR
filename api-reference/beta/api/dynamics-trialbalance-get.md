---
title: Obter trialBalance
description: Obtém um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f758a8c19cafa72c677a4115f1f1d1059e3a2bd6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008070"
---
# <a name="get-trialbalance"></a><span data-ttu-id="cdb26-103">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="cdb26-103">Get trialBalance</span></span>

<span data-ttu-id="cdb26-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cdb26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdb26-105">Recupere as propriedades e os relacionamentos de um objeto de relatório de balancete para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="cdb26-105">Retrieve the properties and relationships of a trial balance report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdb26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdb26-106">Permissions</span></span>
<span data-ttu-id="cdb26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdb26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdb26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdb26-109">Permission type</span></span> |<span data-ttu-id="cdb26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdb26-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cdb26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdb26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdb26-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdb26-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cdb26-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cdb26-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cdb26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdb26-114">Not supported.</span></span>|
|<span data-ttu-id="cdb26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdb26-115">Application</span></span>|<span data-ttu-id="cdb26-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdb26-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdb26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdb26-117">HTTP request</span></span>
```
GET /financials/companies/{id}/trialBalance
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdb26-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cdb26-118">Optional query parameters</span></span>
<span data-ttu-id="cdb26-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdb26-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdb26-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdb26-120">Request headers</span></span>
|<span data-ttu-id="cdb26-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdb26-121">Header</span></span>|<span data-ttu-id="cdb26-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cdb26-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="cdb26-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdb26-123">Authorization</span></span>  |<span data-ttu-id="cdb26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdb26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdb26-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdb26-126">Request body</span></span>
<span data-ttu-id="cdb26-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdb26-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdb26-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdb26-128">Response</span></span>
<span data-ttu-id="cdb26-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **trialBalance** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdb26-129">If successful, this method returns a `200 OK` response code and a **trialBalance** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdb26-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdb26-130">Example</span></span>

<span data-ttu-id="cdb26-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="cdb26-131">**Request**</span></span>

<span data-ttu-id="cdb26-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdb26-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/trialBalance?$orderby number&$filter=dateFilter ge 2019-01-01 and dateFilter le 2019-12-31
```

<span data-ttu-id="cdb26-133">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="cdb26-133">**Response**</span></span>

<span data-ttu-id="cdb26-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdb26-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="cdb26-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdb26-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cdb26-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdb26-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "number": "1110",
  "accountId": "id-value",
  "accountType": "Posting",
  "display": "Accounts Receivable",
  "totalDebit": "479.00",
  "totalCredit": "0.00",
  "balanceAtDateDebit": "72,893.84",
  "balanceAtDateCredit": "0.00",
  "dateFilter": "2019-12-31"    
}
```



