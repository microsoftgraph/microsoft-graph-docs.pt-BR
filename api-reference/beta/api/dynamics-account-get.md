---
title: Obter contas
description: Obtém um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f9d18867474a637ea1f44ef7046d2b476edd47a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454234"
---
# <a name="get-accounts"></a><span data-ttu-id="837ff-103">Obter contas</span><span class="sxs-lookup"><span data-stu-id="837ff-103">Get accounts</span></span>
<span data-ttu-id="837ff-104">Recupere as propriedades e os relacionamentos de um objeto de conta para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="837ff-104">Retrieve the properties and relationships of an account object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="837ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="837ff-105">Permissions</span></span>
<span data-ttu-id="837ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="837ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="837ff-108">Permission type</span></span> |<span data-ttu-id="837ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="837ff-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="837ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="837ff-110">Delegated (work or school account)</span></span>|<span data-ttu-id="837ff-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837ff-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="837ff-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="837ff-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="837ff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837ff-113">Not supported.</span></span>|
|<span data-ttu-id="837ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="837ff-114">Application</span></span>|<span data-ttu-id="837ff-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837ff-115">Financials.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="837ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="837ff-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/accounts('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="837ff-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="837ff-117">Optional query parameters</span></span>
<span data-ttu-id="837ff-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="837ff-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="837ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="837ff-119">Request headers</span></span>
|<span data-ttu-id="837ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="837ff-120">Header</span></span>|<span data-ttu-id="837ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="837ff-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="837ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="837ff-122">Authorization</span></span>  |<span data-ttu-id="837ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="837ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="837ff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="837ff-125">Request body</span></span>
<span data-ttu-id="837ff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="837ff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="837ff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="837ff-127">Response</span></span>
<span data-ttu-id="837ff-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto Accounts no corpo da resposta. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="837ff-128">If successful, this method returns a `200 OK` response code and an **accounts** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837ff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="837ff-129">Example</span></span>

<span data-ttu-id="837ff-130">**Solicitação** Aqui está um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="837ff-130">**Request** Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/accounts('{id}')
```

<span data-ttu-id="837ff-131">**Response**</span><span class="sxs-lookup"><span data-stu-id="837ff-131">**Response**</span></span>

<span data-ttu-id="837ff-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="837ff-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="837ff-133">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="837ff-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="837ff-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="837ff-134">All the properties will be returned from an actual call.</span></span>

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