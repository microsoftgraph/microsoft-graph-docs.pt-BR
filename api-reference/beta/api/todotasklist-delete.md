---
title: Excluir todoTaskList
description: Exclui um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e43ec8d9a8d758a8b064051b95b0ca8256117c1
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849842"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="d606a-103">Excluir todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d606a-103">Delete todoTaskList</span></span>
<span data-ttu-id="d606a-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="d606a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="d606a-105">Exclui um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="d606a-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d606a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d606a-106">Permissions</span></span>
<span data-ttu-id="d606a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d606a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d606a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d606a-109">Permission type</span></span>|<span data-ttu-id="d606a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d606a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d606a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d606a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d606a-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d606a-112">Tasks.Read</span></span>|
|<span data-ttu-id="d606a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d606a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d606a-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d606a-114">Tasks.Read</span></span>|
|<span data-ttu-id="d606a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d606a-115">Application</span></span>|<span data-ttu-id="d606a-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d606a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d606a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d606a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="d606a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d606a-118">Request headers</span></span>
|<span data-ttu-id="d606a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d606a-119">Name</span></span>|<span data-ttu-id="d606a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d606a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d606a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d606a-121">Authorization</span></span>|<span data-ttu-id="d606a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d606a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d606a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d606a-124">Request body</span></span>
<span data-ttu-id="d606a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d606a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d606a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d606a-126">Response</span></span>

<span data-ttu-id="d606a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d606a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d606a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d606a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d606a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d606a-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```


### <a name="response"></a><span data-ttu-id="d606a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d606a-130">Response</span></span>
<span data-ttu-id="d606a-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d606a-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

