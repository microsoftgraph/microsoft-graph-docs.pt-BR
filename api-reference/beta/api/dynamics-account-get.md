---
title: Obter contas
description: Obtém um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 19ef71bd9103ffe257d5a0201e1fde322a78dd0c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142204"
---
# <a name="get-accounts"></a><span data-ttu-id="b0be1-103">Obter contas</span><span class="sxs-lookup"><span data-stu-id="b0be1-103">Get accounts</span></span>

<span data-ttu-id="b0be1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0be1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0be1-105">Recupere as propriedades e os relacionamentos de um objeto de conta para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b0be1-105">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0be1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0be1-106">Permissions</span></span>
<span data-ttu-id="b0be1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b0be1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b0be1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0be1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0be1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0be1-109">Permission type</span></span> |<span data-ttu-id="b0be1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0be1-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b0be1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0be1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0be1-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0be1-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b0be1-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b0be1-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b0be1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0be1-114">Not supported.</span></span>|
|<span data-ttu-id="b0be1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0be1-115">Application</span></span>|<span data-ttu-id="b0be1-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0be1-116">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="b0be1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0be1-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0be1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0be1-118">Optional query parameters</span></span>
<span data-ttu-id="b0be1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0be1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0be1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0be1-120">Request headers</span></span>
|<span data-ttu-id="b0be1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0be1-121">Header</span></span>|<span data-ttu-id="b0be1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0be1-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="b0be1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0be1-123">Authorization</span></span>  |<span data-ttu-id="b0be1-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b0be1-124">Bearer {token}.</span></span> <span data-ttu-id="b0be1-125">Required.</span><span class="sxs-lookup"><span data-stu-id="b0be1-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0be1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0be1-126">Request body</span></span>
<span data-ttu-id="b0be1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0be1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0be1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0be1-128">Response</span></span>
<span data-ttu-id="b0be1-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **accounts** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0be1-129">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0be1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0be1-130">Example</span></span>

<span data-ttu-id="b0be1-131">**Solicitação** Aqui está um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0be1-131">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="b0be1-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="b0be1-132">**Response**</span></span>

<span data-ttu-id="b0be1-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0be1-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="b0be1-134">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b0be1-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b0be1-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0be1-135">All the properties will be returned from an actual call.</span></span>

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
