---
title: Obter taxAreas
description: Obtém um objeto de área fiscal no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: be5f7d436fa219c414f12682679cdfd964ef3ec4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044946"
---
# <a name="get-taxareas"></a><span data-ttu-id="661db-103">Obter taxAreas</span><span class="sxs-lookup"><span data-stu-id="661db-103">Get taxAreas</span></span>

<span data-ttu-id="661db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="661db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="661db-105">Recupere as propriedades e as relações de um objeto de área fiscal do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="661db-105">Retrieve the properties and relationships of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="661db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="661db-106">Permissions</span></span>
<span data-ttu-id="661db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="661db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="661db-109">Permission type</span></span> |<span data-ttu-id="661db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="661db-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="661db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="661db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="661db-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661db-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="661db-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="661db-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="661db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="661db-114">Not supported.</span></span>|
|<span data-ttu-id="661db-115">Application</span><span class="sxs-lookup"><span data-stu-id="661db-115">Application</span></span>|<span data-ttu-id="661db-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661db-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="661db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="661db-117">HTTP request</span></span>

```
GET /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="661db-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="661db-118">Optional query parameters</span></span>
<span data-ttu-id="661db-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="661db-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="661db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="661db-120">Request headers</span></span>
|<span data-ttu-id="661db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="661db-121">Header</span></span>|<span data-ttu-id="661db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="661db-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="661db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="661db-123">Authorization</span></span>  |<span data-ttu-id="661db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="661db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="661db-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="661db-126">Request body</span></span>
<span data-ttu-id="661db-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="661db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="661db-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="661db-128">Response</span></span>
<span data-ttu-id="661db-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto **taxAreas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="661db-129">If successful, this method returns a `200 OK` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="661db-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="661db-130">Example</span></span>

<span data-ttu-id="661db-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="661db-131">**Request**</span></span>

<span data-ttu-id="661db-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="661db-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="661db-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="661db-133">**Response**</span></span>

<span data-ttu-id="661db-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="661db-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="661db-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="661db-135">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```



