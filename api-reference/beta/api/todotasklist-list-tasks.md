---
title: Listar tarefas concluídas
description: Obter os recursos todoTask da propriedade de navegação de tarefas de um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 35e680b4189cf74b22b6f1500c7fe48882c5fd9b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873273"
---
# <a name="list-tasks"></a><span data-ttu-id="d6e86-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d6e86-103">List tasks</span></span>
<span data-ttu-id="d6e86-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="d6e86-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="d6e86-105">Obter os **recursos todoTask** da **propriedade de navegação** tarefas de um [todoTaskList especificado.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="d6e86-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6e86-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6e86-106">Permissions</span></span>
<span data-ttu-id="d6e86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6e86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e86-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6e86-109">Permission type</span></span>|<span data-ttu-id="d6e86-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6e86-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6e86-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6e86-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6e86-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e86-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d6e86-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6e86-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6e86-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e86-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d6e86-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6e86-115">Application</span></span>|<span data-ttu-id="d6e86-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d6e86-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6e86-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e86-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6e86-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6e86-118">Optional query parameters</span></span>
<span data-ttu-id="d6e86-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6e86-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d6e86-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d6e86-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6e86-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e86-121">Request headers</span></span>
|<span data-ttu-id="d6e86-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d6e86-122">Name</span></span>|<span data-ttu-id="d6e86-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6e86-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6e86-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6e86-124">Authorization</span></span>|<span data-ttu-id="d6e86-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6e86-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e86-127">Request body</span></span>
<span data-ttu-id="d6e86-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6e86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6e86-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e86-129">Response</span></span>

<span data-ttu-id="d6e86-130">Se bem-sucedido, este método retorna um código de resposta e `200 OK` uma coleção de objetos [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6e86-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6e86-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6e86-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6e86-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6e86-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6e86-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e86-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```
# <a name="c"></a>[<span data-ttu-id="d6e86-134">C#</span><span class="sxs-lookup"><span data-stu-id="d6e86-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6e86-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6e86-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6e86-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6e86-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6e86-137">Java</span><span class="sxs-lookup"><span data-stu-id="d6e86-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d6e86-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6e86-138">Response</span></span>
<span data-ttu-id="d6e86-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6e86-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



