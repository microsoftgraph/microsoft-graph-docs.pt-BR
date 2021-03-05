---
title: Obter agedAccountsReceivable
description: Obtém um objeto de contas a receber de contas envelhecidas no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
doc_type: apiPageType
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 88f095439d159826aec1edebf9caf7baf2a66454
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471366"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="4daf4-103">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="4daf4-103">Get agedAccountsReceivable</span></span>

<span data-ttu-id="4daf4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4daf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4daf4-105">Recupere as propriedades e as relações de um objeto de relatório de contas a receber do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="4daf4-105">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4daf4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4daf4-106">Permissions</span></span>
<span data-ttu-id="4daf4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4daf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4daf4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4daf4-109">Permission type</span></span> |<span data-ttu-id="4daf4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4daf4-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4daf4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4daf4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4daf4-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4daf4-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4daf4-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4daf4-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4daf4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4daf4-114">Not supported.</span></span>|
|<span data-ttu-id="4daf4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4daf4-115">Application</span></span>|<span data-ttu-id="4daf4-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4daf4-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4daf4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4daf4-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4daf4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4daf4-118">Optional query parameters</span></span>
<span data-ttu-id="4daf4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4daf4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4daf4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4daf4-120">Request headers</span></span>
|<span data-ttu-id="4daf4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4daf4-121">Header</span></span>|<span data-ttu-id="4daf4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4daf4-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="4daf4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4daf4-123">Authorization</span></span>  |<span data-ttu-id="4daf4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4daf4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4daf4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4daf4-126">Request body</span></span>
<span data-ttu-id="4daf4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4daf4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4daf4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4daf4-128">Response</span></span>
<span data-ttu-id="4daf4-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **objeto agedAccountsReceivable** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4daf4-129">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4daf4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4daf4-130">Example</span></span>

<span data-ttu-id="4daf4-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4daf4-131">**Request**</span></span>

<span data-ttu-id="4daf4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4daf4-132">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="4daf4-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="4daf4-133">**Response**</span></span>

<span data-ttu-id="4daf4-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4daf4-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="4daf4-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4daf4-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4daf4-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4daf4-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "customerId": "id-value",
  "customerNumber": "30000",
  "name": "Relecloud",
  "currencyCode": "USD",
  "balanceDue": 349615.45,
  "currentAmount": 0,
  "period1Amount": 349615.45,
  "period2Amount": 0,
  "period3Amount": 0,
  "agedAsOfDate": "2017-04-25",
  "periodLengthFilter": "3M"   
}
```


