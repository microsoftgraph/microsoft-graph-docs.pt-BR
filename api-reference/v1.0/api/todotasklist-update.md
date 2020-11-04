---
title: Atualizar todoTaskList
description: Atualiza as propriedades de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 22e581b2a16f0b16df7de8c2465c2360e55f4be3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904389"
---
# <a name="update-todotasklist"></a><span data-ttu-id="570b5-103">Atualizar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="570b5-103">Update todoTaskList</span></span>
<span data-ttu-id="570b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="570b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="570b5-105">Atualiza as propriedades de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="570b5-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="570b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="570b5-106">Permissions</span></span>
<span data-ttu-id="570b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="570b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="570b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="570b5-109">Permission type</span></span>|<span data-ttu-id="570b5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="570b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="570b5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="570b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="570b5-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="570b5-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="570b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="570b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="570b5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="570b5-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="570b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="570b5-115">Application</span></span>|<span data-ttu-id="570b5-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="570b5-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="570b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="570b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="570b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="570b5-118">Request headers</span></span>
|<span data-ttu-id="570b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="570b5-119">Name</span></span>|<span data-ttu-id="570b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="570b5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="570b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="570b5-121">Authorization</span></span>|<span data-ttu-id="570b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="570b5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="570b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="570b5-124">Content-Type</span></span>|<span data-ttu-id="570b5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="570b5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="570b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="570b5-127">Request body</span></span>
<span data-ttu-id="570b5-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="570b5-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="570b5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="570b5-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="570b5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="570b5-130">Property</span></span>|<span data-ttu-id="570b5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="570b5-131">Type</span></span>|<span data-ttu-id="570b5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="570b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="570b5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="570b5-133">displayName</span></span>|<span data-ttu-id="570b5-134">String</span><span class="sxs-lookup"><span data-stu-id="570b5-134">String</span></span>|<span data-ttu-id="570b5-135">Campo que indica o título atualizado da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="570b5-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="570b5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="570b5-136">Response</span></span>

<span data-ttu-id="570b5-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="570b5-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="570b5-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="570b5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="570b5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="570b5-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="570b5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="570b5-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan"
}
```
# <a name="c"></a>[<span data-ttu-id="570b5-141">C#</span><span class="sxs-lookup"><span data-stu-id="570b5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="570b5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="570b5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="570b5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="570b5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="570b5-144">Java</span><span class="sxs-lookup"><span data-stu-id="570b5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="570b5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="570b5-145">Response</span></span>
<span data-ttu-id="570b5-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="570b5-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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



