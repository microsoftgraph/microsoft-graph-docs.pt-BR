---
title: Atualizar todoTaskList
description: Atualiza as propriedades de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe6a11f889978cd22807816f61be1c85ab7ec912
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873115"
---
# <a name="update-todotasklist"></a><span data-ttu-id="b4d1f-103">Atualizar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="b4d1f-103">Update todoTaskList</span></span>
<span data-ttu-id="b4d1f-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="b4d1f-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="b4d1f-105">Atualiza as propriedades de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="b4d1f-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d1f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4d1f-106">Permissions</span></span>
<span data-ttu-id="b4d1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d1f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4d1f-109">Permission type</span></span>|<span data-ttu-id="b4d1f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4d1f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4d1f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4d1f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4d1f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4d1f-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b4d1f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4d1f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4d1f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4d1f-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b4d1f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4d1f-115">Application</span></span>|<span data-ttu-id="b4d1f-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b4d1f-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4d1f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d1f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="b4d1f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d1f-118">Request headers</span></span>
|<span data-ttu-id="b4d1f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b4d1f-119">Name</span></span>|<span data-ttu-id="b4d1f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d1f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4d1f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4d1f-121">Authorization</span></span>|<span data-ttu-id="b4d1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b4d1f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4d1f-124">Content-Type</span></span>|<span data-ttu-id="b4d1f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d1f-127">Request body</span></span>
<span data-ttu-id="b4d1f-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="b4d1f-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="b4d1f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="b4d1f-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="b4d1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4d1f-130">Property</span></span>|<span data-ttu-id="b4d1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4d1f-131">Type</span></span>|<span data-ttu-id="b4d1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d1f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b4d1f-133">displayName</span></span>|<span data-ttu-id="b4d1f-134">String</span><span class="sxs-lookup"><span data-stu-id="b4d1f-134">String</span></span>|<span data-ttu-id="b4d1f-135">Campo que indica o título atualizado da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b4d1f-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="b4d1f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d1f-136">Response</span></span>

<span data-ttu-id="b4d1f-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4d1f-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4d1f-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4d1f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4d1f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4d1f-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b4d1f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d1f-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b4d1f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4d1f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b4d1f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4d1f-142">Response</span></span>
<span data-ttu-id="b4d1f-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b4d1f-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

