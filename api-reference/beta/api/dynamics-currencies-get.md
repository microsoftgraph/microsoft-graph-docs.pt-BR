---
title: Obter moedas
description: Obtém um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 4657b9a0645aa0a8b241b9a5445fc097bd55390a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791824"
---
# <a name="get-currencies"></a><span data-ttu-id="bd121-103">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="bd121-103">Get currencies</span></span>
<span data-ttu-id="bd121-104">Recupere as propriedades e os relacionamentos de um objeto Currency para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="bd121-104">Retrieve the properties and relationships of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd121-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd121-105">Permissions</span></span>
<span data-ttu-id="bd121-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd121-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd121-108">Permission type</span></span> |<span data-ttu-id="bd121-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd121-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bd121-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd121-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bd121-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd121-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bd121-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bd121-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bd121-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd121-113">Not supported.</span></span>|
|<span data-ttu-id="bd121-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd121-114">Application</span></span>|<span data-ttu-id="bd121-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd121-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd121-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd121-116">HTTP request</span></span>

```
GET /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd121-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd121-117">Optional query parameters</span></span>
<span data-ttu-id="bd121-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd121-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd121-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd121-119">Request headers</span></span>
|<span data-ttu-id="bd121-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd121-120">Header</span></span>|<span data-ttu-id="bd121-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bd121-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="bd121-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd121-122">Authorization</span></span>  |<span data-ttu-id="bd121-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd121-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd121-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd121-125">Request body</span></span>
<span data-ttu-id="bd121-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd121-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd121-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd121-127">Response</span></span>
<span data-ttu-id="bd121-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **moedas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd121-128">If successful, this method returns a `200 OK` response code and a **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd121-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd121-129">Example</span></span>

<span data-ttu-id="bd121-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="bd121-130">**Request**</span></span>

<span data-ttu-id="bd121-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd121-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

<span data-ttu-id="bd121-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="bd121-132">**Response**</span></span>

<span data-ttu-id="bd121-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd121-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="bd121-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bd121-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd121-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd121-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "US",
  "displayName": "US Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:05:09.003Z"
}
```
