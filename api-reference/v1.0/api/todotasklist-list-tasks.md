---
title: Listar tarefas pendentes
description: Obtenha os recursos todoTask da propriedade de navegação Tasks de um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f89a1c97de8410be7d77cc7fb32e2a2e2d33a0c8
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903817"
---
# <a name="list-tasks"></a><span data-ttu-id="7e6aa-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="7e6aa-103">List tasks</span></span>
<span data-ttu-id="7e6aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e6aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e6aa-105">Obtenha os recursos **todoTask** da propriedade de navegação **Tasks** de um [todoTaskList](../resources/todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e6aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e6aa-106">Permissions</span></span>
<span data-ttu-id="7e6aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e6aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e6aa-109">Permission type</span></span>|<span data-ttu-id="7e6aa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e6aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e6aa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e6aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e6aa-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e6aa-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7e6aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e6aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e6aa-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e6aa-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7e6aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e6aa-115">Application</span></span>|<span data-ttu-id="7e6aa-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7e6aa-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e6aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e6aa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e6aa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e6aa-118">Optional query parameters</span></span>
<span data-ttu-id="7e6aa-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7e6aa-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7e6aa-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e6aa-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6aa-121">Request headers</span></span>
|<span data-ttu-id="7e6aa-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7e6aa-122">Name</span></span>|<span data-ttu-id="7e6aa-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e6aa-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7e6aa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e6aa-124">Authorization</span></span>|<span data-ttu-id="7e6aa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e6aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6aa-127">Request body</span></span>
<span data-ttu-id="7e6aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e6aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e6aa-129">Response</span></span>

<span data-ttu-id="7e6aa-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e6aa-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e6aa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e6aa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6aa-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7e6aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e6aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```
# <a name="c"></a>[<span data-ttu-id="7e6aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="7e6aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e6aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e6aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e6aa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e6aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e6aa-137">Java</span><span class="sxs-lookup"><span data-stu-id="7e6aa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7e6aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e6aa-138">Response</span></span>
<span data-ttu-id="7e6aa-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e6aa-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAgdhkVw==\"",
         "importance":"low",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"Linked entity new task 1",
         "createdDateTime":"2020-07-08T11:15:19.9359889Z",
         "lastModifiedDateTime":"2020-07-08T11:15:20.0614375Z",
         "id":"AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD",
         "body":{
            "content":"",
            "contentType":"text"
         },
         "linkedResources@odata.context":"https://graph.microsoft.com/beta/$metadata#users('todoservicetest2412201901%40outlook.com')/todo/lists('35e2-35e2-721a-e235-1a72e2351a7')/tasks('AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD')/linkedResources",
         "linkedResources":[
            {
               "applicationName":"Partner App Name",
               "displayName":"Partner App Name",
               "externalId":"teset1243434",
               "id":"30911960-7321-4cba-9ba0-cdb68e2984c7"
            }
         ]
      }
   ]
}
```



