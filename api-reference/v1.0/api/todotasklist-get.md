---
title: Obter todoTaskList
description: Leia as propriedades e os relacionamentos de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7aced0d3e023eacfde6faaecc8c63836bbb44b7
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797211"
---
# <a name="get-todotasklist"></a><span data-ttu-id="9f26c-103">Obter todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9f26c-103">Get todoTaskList</span></span>
<span data-ttu-id="9f26c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f26c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f26c-105">Leia as propriedades e os relacionamentos de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="9f26c-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f26c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f26c-106">Permissions</span></span>
<span data-ttu-id="9f26c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f26c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f26c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f26c-109">Permission type</span></span>|<span data-ttu-id="9f26c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f26c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f26c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f26c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f26c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f26c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9f26c-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="9f26c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f26c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f26c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9f26c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f26c-115">Application</span></span>|<span data-ttu-id="9f26c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f26c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f26c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f26c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f26c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f26c-118">Optional query parameters</span></span>
<span data-ttu-id="9f26c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f26c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f26c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f26c-120">Request headers</span></span>
|<span data-ttu-id="9f26c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9f26c-121">Name</span></span>|<span data-ttu-id="9f26c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f26c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f26c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f26c-123">Authorization</span></span>|<span data-ttu-id="9f26c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f26c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f26c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f26c-126">Request body</span></span>
<span data-ttu-id="9f26c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f26c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f26c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f26c-128">Response</span></span>

<span data-ttu-id="9f26c-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f26c-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f26c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f26c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f26c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f26c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAAABrJAAA=
```


### <a name="response"></a><span data-ttu-id="9f26c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f26c-132">Response</span></span>
><span data-ttu-id="9f26c-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9f26c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.todoTaskList",
    "id": "5daae1ed-e1ed-5daa-ede1-aa5dede1aa5d",
    "displayName": "Monthly tasks",
    "isOwner": "true",
    "isShared": "false",
    "wellknownListName": "defaultList"
  }
}
```



