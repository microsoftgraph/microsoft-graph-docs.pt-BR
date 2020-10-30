---
title: List lists
description: Obtenha uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20059bac4108c6736e09f41d9e41876c566f8865
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797216"
---
# <a name="list-lists"></a><span data-ttu-id="68c8d-103">List lists</span><span class="sxs-lookup"><span data-stu-id="68c8d-103">List lists</span></span>
<span data-ttu-id="68c8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68c8d-105">Obtenha uma lista dos objetos [todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="68c8d-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="68c8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68c8d-106">Permissions</span></span>
<span data-ttu-id="68c8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68c8d-109">Permission type</span></span>|<span data-ttu-id="68c8d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68c8d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68c8d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68c8d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68c8d-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68c8d-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="68c8d-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="68c8d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68c8d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68c8d-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="68c8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68c8d-115">Application</span></span>|<span data-ttu-id="68c8d-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="68c8d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="68c8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68c8d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68c8d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68c8d-118">Optional query parameters</span></span>
<span data-ttu-id="68c8d-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68c8d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="68c8d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="68c8d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="68c8d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68c8d-121">Request headers</span></span>
|<span data-ttu-id="68c8d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="68c8d-122">Name</span></span>|<span data-ttu-id="68c8d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c8d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68c8d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="68c8d-124">Authorization</span></span>|<span data-ttu-id="68c8d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68c8d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68c8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68c8d-127">Request body</span></span>
<span data-ttu-id="68c8d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68c8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68c8d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c8d-129">Response</span></span>

<span data-ttu-id="68c8d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68c8d-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68c8d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68c8d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68c8d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c8d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists
```


### <a name="response"></a><span data-ttu-id="68c8d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c8d-133">Response</span></span>
<span data-ttu-id="68c8d-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="68c8d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAAABrJAAA=",
      "displayName": "Tasks",
      "isOwner": true,
      "isShared": false,
      "wellknownListName": "defaultList"
    },
        {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAEFTTrJAAA=",
      "displayName": "Monthly Tasks",
      "isOwner":true,
      "isShared": false,
      "wellknownListName": "none"
    }
  ]
}
```



