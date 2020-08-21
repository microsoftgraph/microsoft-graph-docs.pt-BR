---
title: Atualizar todoTaskList
description: Atualiza as propriedades de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bedcf564fdc470a6bfcf1dacafe2efa82694e0ed
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849831"
---
# <a name="update-todotasklist"></a><span data-ttu-id="1c489-103">Atualizar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="1c489-103">Update todoTaskList</span></span>
<span data-ttu-id="1c489-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="1c489-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="1c489-105">Atualiza as propriedades de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="1c489-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c489-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c489-106">Permissions</span></span>
<span data-ttu-id="1c489-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c489-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c489-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c489-109">Permission type</span></span>|<span data-ttu-id="1c489-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c489-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c489-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c489-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c489-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c489-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1c489-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c489-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c489-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c489-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1c489-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c489-115">Application</span></span>|<span data-ttu-id="1c489-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1c489-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c489-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c489-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="1c489-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c489-118">Request headers</span></span>
|<span data-ttu-id="1c489-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1c489-119">Name</span></span>|<span data-ttu-id="1c489-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c489-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c489-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c489-121">Authorization</span></span>|<span data-ttu-id="1c489-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c489-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1c489-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c489-124">Content-Type</span></span>|<span data-ttu-id="1c489-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c489-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c489-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c489-127">Request body</span></span>
<span data-ttu-id="1c489-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="1c489-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="1c489-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTaskList](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="1c489-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="1c489-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c489-130">Property</span></span>|<span data-ttu-id="1c489-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c489-131">Type</span></span>|<span data-ttu-id="1c489-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c489-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c489-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1c489-133">displayName</span></span>|<span data-ttu-id="1c489-134">String</span><span class="sxs-lookup"><span data-stu-id="1c489-134">String</span></span>|<span data-ttu-id="1c489-135">Campo que indica o título atualizado da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="1c489-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="1c489-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c489-136">Response</span></span>

<span data-ttu-id="1c489-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c489-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c489-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c489-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c489-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c489-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="1c489-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c489-140">Response</span></span>
<span data-ttu-id="1c489-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c489-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

