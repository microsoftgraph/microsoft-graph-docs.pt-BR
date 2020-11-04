---
title: Criar todoTaskList
description: Criar um novo objeto Lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ffc3b2af61aeb4e37f687f85d35311a8c0adcae1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904077"
---
# <a name="create-todotasklist"></a><span data-ttu-id="76e6f-103">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="76e6f-103">Create todoTaskList</span></span>
<span data-ttu-id="76e6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76e6f-105">Criar um novo objeto Lists.</span><span class="sxs-lookup"><span data-stu-id="76e6f-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="76e6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="76e6f-106">Permissions</span></span>
<span data-ttu-id="76e6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76e6f-109">Permission type</span></span>|<span data-ttu-id="76e6f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76e6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76e6f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76e6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76e6f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76e6f-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="76e6f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76e6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76e6f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76e6f-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="76e6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76e6f-115">Application</span></span>|<span data-ttu-id="76e6f-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="76e6f-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="76e6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76e6f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="76e6f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76e6f-118">Request headers</span></span>
|<span data-ttu-id="76e6f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="76e6f-119">Name</span></span>|<span data-ttu-id="76e6f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e6f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="76e6f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="76e6f-121">Authorization</span></span>|<span data-ttu-id="76e6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76e6f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="76e6f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76e6f-124">Content-Type</span></span>|<span data-ttu-id="76e6f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76e6f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76e6f-127">Request body</span></span>
<span data-ttu-id="76e6f-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="76e6f-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="76e6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="76e6f-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="76e6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76e6f-130">Property</span></span>|<span data-ttu-id="76e6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76e6f-131">Type</span></span>|<span data-ttu-id="76e6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76e6f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="76e6f-133">displayName</span></span>|<span data-ttu-id="76e6f-134">String</span><span class="sxs-lookup"><span data-stu-id="76e6f-134">String</span></span>|<span data-ttu-id="76e6f-135">Campo indicando o título da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="76e6f-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="76e6f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e6f-136">Response</span></span>

<span data-ttu-id="76e6f-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76e6f-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76e6f-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="76e6f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76e6f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76e6f-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="76e6f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="76e6f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_todotasklist_from_lists"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists
Content-Type: application/json
Content-length: 60

{
  "displayName": "Travel items"
}
```
# <a name="c"></a>[<span data-ttu-id="76e6f-141">C#</span><span class="sxs-lookup"><span data-stu-id="76e6f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76e6f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76e6f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76e6f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76e6f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76e6f-144">Java</span><span class="sxs-lookup"><span data-stu-id="76e6f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotasklist-from-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="76e6f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e6f-145">Response</span></span>
<span data-ttu-id="76e6f-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="76e6f-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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


