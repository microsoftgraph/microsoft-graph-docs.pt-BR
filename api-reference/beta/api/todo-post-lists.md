---
title: Criar todoTaskList
description: Criar um novo objeto de listas.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 92242d0973b3d47af0126f6fefb093d258f46d74
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874078"
---
# <a name="create-todotasklist"></a><span data-ttu-id="1653a-103">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="1653a-103">Create todoTaskList</span></span>
<span data-ttu-id="1653a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1653a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1653a-105">Criar um novo objeto de listas.</span><span class="sxs-lookup"><span data-stu-id="1653a-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1653a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1653a-106">Permissions</span></span>
<span data-ttu-id="1653a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1653a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1653a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1653a-109">Permission type</span></span>|<span data-ttu-id="1653a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1653a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1653a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1653a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1653a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1653a-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1653a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1653a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1653a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1653a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1653a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1653a-115">Application</span></span>|<span data-ttu-id="1653a-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1653a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1653a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1653a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="1653a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1653a-118">Request headers</span></span>
|<span data-ttu-id="1653a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1653a-119">Name</span></span>|<span data-ttu-id="1653a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1653a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1653a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1653a-121">Authorization</span></span>|<span data-ttu-id="1653a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1653a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1653a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1653a-124">Content-Type</span></span>|<span data-ttu-id="1653a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1653a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1653a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1653a-127">Request body</span></span>
<span data-ttu-id="1653a-128">No corpo da solicitação, fornece uma representação JSON do [objeto todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="1653a-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="1653a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="1653a-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="1653a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1653a-130">Property</span></span>|<span data-ttu-id="1653a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1653a-131">Type</span></span>|<span data-ttu-id="1653a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1653a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1653a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1653a-133">displayName</span></span>|<span data-ttu-id="1653a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1653a-134">String</span></span>|<span data-ttu-id="1653a-135">Campo que indica o título da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="1653a-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="1653a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1653a-136">Response</span></span>

<span data-ttu-id="1653a-137">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1653a-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1653a-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1653a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1653a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1653a-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1653a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1653a-140">HTTP</span></span>](#tab/http)
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
  "displayName": "Travel items"
}
```
# <a name="javascript"></a>[<span data-ttu-id="1653a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1653a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1653a-142">C#</span><span class="sxs-lookup"><span data-stu-id="1653a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1653a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1653a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1653a-144">Java</span><span class="sxs-lookup"><span data-stu-id="1653a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotasklist-from-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1653a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1653a-145">Response</span></span>
<span data-ttu-id="1653a-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1653a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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


