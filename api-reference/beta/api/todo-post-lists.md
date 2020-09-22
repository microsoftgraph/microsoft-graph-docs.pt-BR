---
title: Criar todoTaskList
description: Criar um novo objeto Lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 91b7211e15d02dd97101ca513be8cb85147c23a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010441"
---
# <a name="create-todotasklist"></a><span data-ttu-id="f0053-103">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="f0053-103">Create todoTaskList</span></span>
<span data-ttu-id="f0053-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f0053-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0053-105">Criar um novo objeto Lists.</span><span class="sxs-lookup"><span data-stu-id="f0053-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0053-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0053-106">Permissions</span></span>
<span data-ttu-id="f0053-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0053-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0053-109">Permission type</span></span>|<span data-ttu-id="f0053-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0053-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0053-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0053-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0053-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0053-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f0053-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0053-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0053-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0053-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f0053-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0053-115">Application</span></span>|<span data-ttu-id="f0053-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f0053-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0053-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0053-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="f0053-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0053-118">Request headers</span></span>
|<span data-ttu-id="f0053-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f0053-119">Name</span></span>|<span data-ttu-id="f0053-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0053-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0053-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0053-121">Authorization</span></span>|<span data-ttu-id="f0053-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0053-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f0053-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0053-124">Content-Type</span></span>|<span data-ttu-id="f0053-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0053-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0053-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0053-127">Request body</span></span>
<span data-ttu-id="f0053-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="f0053-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="f0053-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="f0053-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="f0053-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0053-130">Property</span></span>|<span data-ttu-id="f0053-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0053-131">Type</span></span>|<span data-ttu-id="f0053-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0053-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0053-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f0053-133">displayName</span></span>|<span data-ttu-id="f0053-134">String</span><span class="sxs-lookup"><span data-stu-id="f0053-134">String</span></span>|<span data-ttu-id="f0053-135">Campo indicando o título da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f0053-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="f0053-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0053-136">Response</span></span>

<span data-ttu-id="f0053-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0053-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0053-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0053-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0053-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0053-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f0053-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0053-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_todotasklist_from_lists"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists
Content-Type: application/json
Content-length: 60

{
  "displayName": "Travel items",
}
```
# <a name="javascript"></a>[<span data-ttu-id="f0053-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0053-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f0053-142">C#</span><span class="sxs-lookup"><span data-stu-id="f0053-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0053-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0053-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f0053-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0053-144">Response</span></span>
<span data-ttu-id="f0053-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0053-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Travel items",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```


