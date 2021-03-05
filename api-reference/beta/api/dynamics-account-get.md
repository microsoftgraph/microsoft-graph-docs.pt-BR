---
title: Obter contas
description: Obtém um objeto de conta no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6af282938adaf801046164b94270bcf2e60d98a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471373"
---
# <a name="get-accounts"></a><span data-ttu-id="0efaa-103">Obter contas</span><span class="sxs-lookup"><span data-stu-id="0efaa-103">Get accounts</span></span>

<span data-ttu-id="0efaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0efaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0efaa-105">Recupere as propriedades e as relações de um objeto de conta do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="0efaa-105">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0efaa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0efaa-106">Permissions</span></span>
<span data-ttu-id="0efaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0efaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0efaa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0efaa-109">Permission type</span></span> |<span data-ttu-id="0efaa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0efaa-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0efaa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0efaa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0efaa-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0efaa-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0efaa-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0efaa-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0efaa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0efaa-114">Not supported.</span></span>|
|<span data-ttu-id="0efaa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0efaa-115">Application</span></span>|<span data-ttu-id="0efaa-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0efaa-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="0efaa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0efaa-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0efaa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0efaa-118">Optional query parameters</span></span>
<span data-ttu-id="0efaa-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0efaa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0efaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0efaa-120">Request headers</span></span>
|<span data-ttu-id="0efaa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0efaa-121">Header</span></span>|<span data-ttu-id="0efaa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0efaa-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="0efaa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0efaa-123">Authorization</span></span>  |<span data-ttu-id="0efaa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0efaa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0efaa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0efaa-126">Request body</span></span>
<span data-ttu-id="0efaa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0efaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0efaa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0efaa-128">Response</span></span>
<span data-ttu-id="0efaa-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **accounts** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0efaa-129">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0efaa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0efaa-130">Example</span></span>

<span data-ttu-id="0efaa-131">**Solicitação** Aqui está um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0efaa-131">**Request** Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="0efaa-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="0efaa-132">**Response**</span></span>

<span data-ttu-id="0efaa-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0efaa-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="0efaa-134">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0efaa-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0efaa-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0efaa-135">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "id-value",
    "number": "10700",
    "displayName": "Inventory",
    "category": "Assets",
    "subCategory": "Inventory",
    "blocked": false,
    "lastModifiedDateTime": "2017-03-15T02:20:58.747Z"
}
```


