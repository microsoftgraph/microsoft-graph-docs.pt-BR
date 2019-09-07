---
title: Obter contas
description: Obtém um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b020d6204a5c99f9b3a49721a3fc327f3314f4f7
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792230"
---
# <a name="get-accounts"></a><span data-ttu-id="3feaf-103">Obter contas</span><span class="sxs-lookup"><span data-stu-id="3feaf-103">Get accounts</span></span>
<span data-ttu-id="3feaf-104">Recupere as propriedades e os relacionamentos de um objeto de conta para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3feaf-104">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3feaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3feaf-105">Permissions</span></span>
<span data-ttu-id="3feaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3feaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3feaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3feaf-108">Permission type</span></span> |<span data-ttu-id="3feaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3feaf-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3feaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3feaf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3feaf-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3feaf-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3feaf-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3feaf-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3feaf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3feaf-113">Not supported.</span></span>|
|<span data-ttu-id="3feaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3feaf-114">Application</span></span>|<span data-ttu-id="3feaf-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3feaf-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="3feaf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3feaf-116">HTTP request</span></span>
```
GET /financials/companies/{id}/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3feaf-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3feaf-117">Optional query parameters</span></span>
<span data-ttu-id="3feaf-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3feaf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3feaf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3feaf-119">Request headers</span></span>
|<span data-ttu-id="3feaf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3feaf-120">Header</span></span>|<span data-ttu-id="3feaf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3feaf-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3feaf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3feaf-122">Authorization</span></span>  |<span data-ttu-id="3feaf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3feaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3feaf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3feaf-125">Request body</span></span>
<span data-ttu-id="3feaf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3feaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3feaf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3feaf-127">Response</span></span>
<span data-ttu-id="3feaf-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **accounts** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3feaf-128">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3feaf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3feaf-129">Example</span></span>

<span data-ttu-id="3feaf-130">**Solicitação** Aqui está um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3feaf-130">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/accounts/{id}
```

<span data-ttu-id="3feaf-131">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="3feaf-131">**Response**</span></span>

<span data-ttu-id="3feaf-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3feaf-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="3feaf-133">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3feaf-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3feaf-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3feaf-134">All the properties will be returned from an actual call.</span></span>

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