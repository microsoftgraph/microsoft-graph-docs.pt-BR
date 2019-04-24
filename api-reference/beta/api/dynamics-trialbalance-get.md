---
title: Obter trialBalance
description: Obtém um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0729155ddef94d28afb0cb0a85fd095931ffdbb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458366"
---
# <a name="get-trialbalance"></a><span data-ttu-id="d1e13-103">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="d1e13-103">Get trialBalance</span></span>
<span data-ttu-id="d1e13-104">Recupere as propriedades e os relacionamentos de um objeto de relatório de balancete para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="d1e13-104">Retrieve the properties and relationships of a trial balance report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1e13-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1e13-105">Permissions</span></span>
<span data-ttu-id="d1e13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e13-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1e13-108">Permission type</span></span> |<span data-ttu-id="d1e13-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1e13-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d1e13-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1e13-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e13-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e13-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d1e13-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d1e13-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d1e13-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1e13-113">Not supported.</span></span>|
|<span data-ttu-id="d1e13-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1e13-114">Application</span></span>|<span data-ttu-id="d1e13-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e13-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1e13-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e13-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/trialBalance
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1e13-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1e13-117">Optional query parameters</span></span>
<span data-ttu-id="d1e13-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1e13-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1e13-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e13-119">Request headers</span></span>
|<span data-ttu-id="d1e13-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1e13-120">Header</span></span>|<span data-ttu-id="d1e13-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d1e13-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="d1e13-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1e13-122">Authorization</span></span>  |<span data-ttu-id="d1e13-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1e13-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1e13-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e13-125">Request body</span></span>
<span data-ttu-id="d1e13-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1e13-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1e13-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1e13-127">Response</span></span>
<span data-ttu-id="d1e13-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **trialBalance** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1e13-128">If successful, this method returns a `200 OK` response code and a **trialBalance** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1e13-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1e13-129">Example</span></span>

<span data-ttu-id="d1e13-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="d1e13-130">**Request**</span></span>

<span data-ttu-id="d1e13-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1e13-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/trialBalance?$orderby number&$filter=dateFilter ge 2019-01-01 and dateFilter le 2019-12-31
```

<span data-ttu-id="d1e13-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="d1e13-132">**Response**</span></span>

<span data-ttu-id="d1e13-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1e13-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="d1e13-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d1e13-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d1e13-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1e13-135">All the properties will be returned from an actual call.</span></span>

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

