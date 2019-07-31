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
ms.openlocfilehash: 3e23ea971ad16d32d3a651259818524870abedc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956846"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="ae702-103">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="ae702-103">Get agedAccountsReceivable</span></span>
<span data-ttu-id="ae702-104">Recupere as propriedades e os relacionamentos de um objeto de relatório de contas a receber antigo para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ae702-104">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae702-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae702-105">Permissions</span></span>
<span data-ttu-id="ae702-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae702-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae702-108">Permission type</span></span> |<span data-ttu-id="ae702-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae702-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="ae702-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae702-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ae702-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae702-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="ae702-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ae702-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ae702-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae702-113">Not supported.</span></span>|
|<span data-ttu-id="ae702-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae702-114">Application</span></span>|<span data-ttu-id="ae702-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae702-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae702-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae702-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae702-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae702-117">Optional query parameters</span></span>
<span data-ttu-id="ae702-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae702-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae702-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae702-119">Request headers</span></span>
|<span data-ttu-id="ae702-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae702-120">Header</span></span>|<span data-ttu-id="ae702-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ae702-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="ae702-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae702-122">Authorization</span></span>  |<span data-ttu-id="ae702-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae702-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae702-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae702-125">Request body</span></span>
<span data-ttu-id="ae702-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae702-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae702-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae702-127">Response</span></span>
<span data-ttu-id="ae702-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **agedAccountsReceivable** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae702-128">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae702-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae702-129">Example</span></span>

<span data-ttu-id="ae702-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="ae702-130">**Request**</span></span>

<span data-ttu-id="ae702-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae702-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="ae702-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="ae702-132">**Response**</span></span>

<span data-ttu-id="ae702-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae702-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="ae702-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae702-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae702-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae702-135">All the properties will be returned from an actual call.</span></span>

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
