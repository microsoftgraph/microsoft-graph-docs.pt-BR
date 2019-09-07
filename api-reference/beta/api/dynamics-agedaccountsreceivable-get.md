---
title: Obter agedAccountsReceivable
description: Obtém um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.author: solsen
doc_type: apiPageType
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 15e29f2cfce50cb2e24e503fc893354fbb94f48a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792216"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="85232-103">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="85232-103">Get agedAccountsReceivable</span></span>
<span data-ttu-id="85232-104">Recupere as propriedades e os relacionamentos de um objeto de relatório de contas a receber antigo para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="85232-104">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="85232-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85232-105">Permissions</span></span>
<span data-ttu-id="85232-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85232-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85232-108">Permission type</span></span> |<span data-ttu-id="85232-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85232-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="85232-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85232-110">Delegated (work or school account)</span></span>|<span data-ttu-id="85232-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85232-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="85232-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="85232-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="85232-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85232-113">Not supported.</span></span>|
|<span data-ttu-id="85232-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85232-114">Application</span></span>|<span data-ttu-id="85232-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85232-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85232-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85232-116">HTTP request</span></span>
```
GET /financials/companies/{id}/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85232-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85232-117">Optional query parameters</span></span>
<span data-ttu-id="85232-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85232-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85232-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85232-119">Request headers</span></span>
|<span data-ttu-id="85232-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85232-120">Header</span></span>|<span data-ttu-id="85232-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85232-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="85232-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85232-122">Authorization</span></span>  |<span data-ttu-id="85232-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85232-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85232-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85232-125">Request body</span></span>
<span data-ttu-id="85232-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85232-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85232-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="85232-127">Response</span></span>
<span data-ttu-id="85232-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **agedAccountsReceivable** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85232-128">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85232-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85232-129">Example</span></span>

<span data-ttu-id="85232-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="85232-130">**Request**</span></span>

<span data-ttu-id="85232-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85232-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="85232-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="85232-132">**Response**</span></span>

<span data-ttu-id="85232-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85232-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="85232-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85232-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85232-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85232-135">All the properties will be returned from an actual call.</span></span>

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
