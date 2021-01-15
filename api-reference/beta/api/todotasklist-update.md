---
title: Atualizar todoTaskList
description: Atualize as propriedades de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 582e9eb65ab0670d1f5c5e735c156e0ac414a19e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873189"
---
# <a name="update-todotasklist"></a><span data-ttu-id="a0652-103">Atualizar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a0652-103">Update todoTaskList</span></span>
<span data-ttu-id="a0652-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a0652-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="a0652-105">Atualize as propriedades de um [objeto todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="a0652-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0652-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0652-106">Permissions</span></span>
<span data-ttu-id="a0652-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0652-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0652-109">Permission type</span></span>|<span data-ttu-id="a0652-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0652-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0652-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0652-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0652-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0652-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a0652-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0652-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0652-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0652-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a0652-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0652-115">Application</span></span>|<span data-ttu-id="a0652-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0652-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0652-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0652-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="a0652-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0652-118">Request headers</span></span>
|<span data-ttu-id="a0652-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a0652-119">Name</span></span>|<span data-ttu-id="a0652-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0652-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0652-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0652-121">Authorization</span></span>|<span data-ttu-id="a0652-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0652-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a0652-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0652-124">Content-Type</span></span>|<span data-ttu-id="a0652-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0652-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0652-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0652-127">Request body</span></span>
<span data-ttu-id="a0652-128">No corpo da solicitação, fornece uma representação JSON do [objeto todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="a0652-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="a0652-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="a0652-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="a0652-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0652-130">Property</span></span>|<span data-ttu-id="a0652-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0652-131">Type</span></span>|<span data-ttu-id="a0652-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0652-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0652-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a0652-133">displayName</span></span>|<span data-ttu-id="a0652-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0652-134">String</span></span>|<span data-ttu-id="a0652-135">Campo que indica o título atualizado da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="a0652-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="a0652-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0652-136">Response</span></span>

<span data-ttu-id="a0652-137">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [todoTaskList](../resources/todotasklist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0652-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0652-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0652-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0652-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0652-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a0652-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0652-140">HTTP</span></span>](#tab/http)
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
  "displayName": "Vacation Plan"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a0652-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0652-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a0652-142">C#</span><span class="sxs-lookup"><span data-stu-id="a0652-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0652-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0652-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0652-144">Java</span><span class="sxs-lookup"><span data-stu-id="a0652-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a0652-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0652-145">Response</span></span>
<span data-ttu-id="a0652-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0652-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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



