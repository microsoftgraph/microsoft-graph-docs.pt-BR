---
title: Listar listas
description: Obtenha uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 87b7cad3f24d8e0db1632edd43454a55d05e64b0
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849858"
---
# <a name="list-lists"></a><span data-ttu-id="f7abf-103">Listar listas</span><span class="sxs-lookup"><span data-stu-id="f7abf-103">List lists</span></span>
<span data-ttu-id="f7abf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7abf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7abf-105">Obtenha uma lista dos objetos [todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f7abf-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7abf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7abf-106">Permissions</span></span>
<span data-ttu-id="f7abf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7abf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7abf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7abf-109">Permission type</span></span>|<span data-ttu-id="f7abf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7abf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7abf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7abf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7abf-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7abf-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7abf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7abf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7abf-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7abf-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7abf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7abf-115">Application</span></span>|<span data-ttu-id="f7abf-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f7abf-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7abf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7abf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7abf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7abf-118">Optional query parameters</span></span>
<span data-ttu-id="f7abf-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7abf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f7abf-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f7abf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7abf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7abf-121">Request headers</span></span>
|<span data-ttu-id="f7abf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7abf-122">Name</span></span>|<span data-ttu-id="f7abf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7abf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7abf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7abf-124">Authorization</span></span>|<span data-ttu-id="f7abf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7abf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7abf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7abf-127">Request body</span></span>
<span data-ttu-id="f7abf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7abf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7abf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7abf-129">Response</span></span>

<span data-ttu-id="f7abf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7abf-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7abf-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7abf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7abf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7abf-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```


### <a name="response"></a><span data-ttu-id="f7abf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7abf-133">Response</span></span>
<span data-ttu-id="f7abf-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7abf-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
