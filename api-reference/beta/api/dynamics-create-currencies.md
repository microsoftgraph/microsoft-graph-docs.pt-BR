---
title: Criar moedas
description: Cria um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 53da84723042439505a91dee3838426db6ced820
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454070"
---
# <a name="create-currencies"></a><span data-ttu-id="94bd1-103">Criar moedas</span><span class="sxs-lookup"><span data-stu-id="94bd1-103">Create currencies</span></span>
<span data-ttu-id="94bd1-104">Criar um objeto Currency no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="94bd1-104">Create a currency object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="94bd1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="94bd1-105">Permissions</span></span>
<span data-ttu-id="94bd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94bd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94bd1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94bd1-108">Permission type</span></span> |<span data-ttu-id="94bd1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94bd1-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="94bd1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94bd1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="94bd1-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94bd1-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="94bd1-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="94bd1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="94bd1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94bd1-113">Not supported.</span></span>|
|<span data-ttu-id="94bd1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94bd1-114">Application</span></span>|<span data-ttu-id="94bd1-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94bd1-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94bd1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94bd1-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/currencies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94bd1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94bd1-117">Optional query parameters</span></span>
<span data-ttu-id="94bd1-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94bd1-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94bd1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94bd1-119">Request headers</span></span>
|<span data-ttu-id="94bd1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94bd1-120">Header</span></span>         |<span data-ttu-id="94bd1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94bd1-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="94bd1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94bd1-122">Authorization</span></span>  |<span data-ttu-id="94bd1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94bd1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="94bd1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94bd1-125">Content-Type</span></span>   |<span data-ttu-id="94bd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94bd1-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="94bd1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94bd1-127">Request body</span></span>
<span data-ttu-id="94bd1-128">No corpo da solicitação, forneça uma representação JSON do objeto **moedas** .</span><span class="sxs-lookup"><span data-stu-id="94bd1-128">In the request body, supply a JSON representation of **currencies** object.</span></span>

## <a name="response"></a><span data-ttu-id="94bd1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94bd1-129">Response</span></span>
<span data-ttu-id="94bd1-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e um objeto de **moedas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94bd1-130">If successful, this method returns ```201 Created``` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94bd1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94bd1-131">Example</span></span>

<span data-ttu-id="94bd1-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="94bd1-132">**Request**</span></span>

<span data-ttu-id="94bd1-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="94bd1-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/currencies
Content-type: application/json

{
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01
}
```

<span data-ttu-id="94bd1-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="94bd1-134">**Response**</span></span>

<span data-ttu-id="94bd1-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94bd1-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="94bd1-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94bd1-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94bd1-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94bd1-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.002Z"
}

```
