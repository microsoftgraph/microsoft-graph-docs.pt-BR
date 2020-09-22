---
title: Atualizar todoTaskList
description: Atualiza as propriedades de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f88e1646d78a045d446db8dea92dbb815345d73f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027437"
---
# <a name="update-todotasklist"></a><span data-ttu-id="e121c-103">Atualizar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="e121c-103">Update todoTaskList</span></span>
<span data-ttu-id="e121c-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="e121c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="e121c-105">Atualiza as propriedades de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="e121c-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e121c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e121c-106">Permissions</span></span>
<span data-ttu-id="e121c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e121c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e121c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e121c-109">Permission type</span></span>|<span data-ttu-id="e121c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e121c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e121c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e121c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e121c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e121c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e121c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e121c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e121c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e121c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e121c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e121c-115">Application</span></span>|<span data-ttu-id="e121c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e121c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e121c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e121c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="e121c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e121c-118">Request headers</span></span>
|<span data-ttu-id="e121c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e121c-119">Name</span></span>|<span data-ttu-id="e121c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e121c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e121c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e121c-121">Authorization</span></span>|<span data-ttu-id="e121c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e121c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e121c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e121c-124">Content-Type</span></span>|<span data-ttu-id="e121c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e121c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e121c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e121c-127">Request body</span></span>
<span data-ttu-id="e121c-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="e121c-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="e121c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="e121c-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="e121c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e121c-130">Property</span></span>|<span data-ttu-id="e121c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e121c-131">Type</span></span>|<span data-ttu-id="e121c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e121c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e121c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e121c-133">displayName</span></span>|<span data-ttu-id="e121c-134">String</span><span class="sxs-lookup"><span data-stu-id="e121c-134">String</span></span>|<span data-ttu-id="e121c-135">Campo que indica o título atualizado da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="e121c-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="e121c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e121c-136">Response</span></span>

<span data-ttu-id="e121c-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e121c-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e121c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e121c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e121c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e121c-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e121c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e121c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan",
}
```
# <a name="javascript"></a>[<span data-ttu-id="e121c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e121c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e121c-142">C#</span><span class="sxs-lookup"><span data-stu-id="e121c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e121c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e121c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e121c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e121c-144">Response</span></span>
<span data-ttu-id="e121c-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e121c-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Vacation Plan",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```



