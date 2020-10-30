---
title: Excluir todoTaskList
description: Exclui um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 83944ea1b4749a556646fe6133facb14e88d612c
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797182"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="ce5b7-103">Excluir todoTaskList</span><span class="sxs-lookup"><span data-stu-id="ce5b7-103">Delete todoTaskList</span></span>
<span data-ttu-id="ce5b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce5b7-105">Exclui um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="ce5b7-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce5b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce5b7-106">Permissions</span></span>
<span data-ttu-id="ce5b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce5b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce5b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce5b7-109">Permission type</span></span>|<span data-ttu-id="ce5b7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce5b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce5b7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce5b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce5b7-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ce5b7-112">Tasks.Read</span></span>|
|<span data-ttu-id="ce5b7-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="ce5b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce5b7-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ce5b7-114">Tasks.Read</span></span>|
|<span data-ttu-id="ce5b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce5b7-115">Application</span></span>|<span data-ttu-id="ce5b7-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ce5b7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce5b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5b7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="ce5b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5b7-118">Request headers</span></span>
|<span data-ttu-id="ce5b7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ce5b7-119">Name</span></span>|<span data-ttu-id="ce5b7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5b7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce5b7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce5b7-121">Authorization</span></span>|<span data-ttu-id="ce5b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5b7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce5b7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5b7-124">Request body</span></span>
<span data-ttu-id="ce5b7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce5b7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce5b7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5b7-126">Response</span></span>

<span data-ttu-id="ce5b7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce5b7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ce5b7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce5b7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce5b7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5b7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```


### <a name="response"></a><span data-ttu-id="ce5b7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5b7-130">Response</span></span>
<span data-ttu-id="ce5b7-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce5b7-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



