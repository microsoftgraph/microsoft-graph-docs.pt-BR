---
title: Listar tarefas pendentes
description: Obtenha os recursos todoTask da propriedade de navegação Tasks de um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 83109dca2506494bf1b9eb77cfb1b70a734a2e40
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849837"
---
# <a name="list-tasks"></a><span data-ttu-id="ee3ba-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="ee3ba-103">List tasks</span></span>
<span data-ttu-id="ee3ba-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="ee3ba-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="ee3ba-105">Obtenha os recursos **todoTask** da propriedade de navegação **Tasks** de um [todoTaskList](../resources/todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee3ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee3ba-106">Permissions</span></span>
<span data-ttu-id="ee3ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee3ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee3ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee3ba-109">Permission type</span></span>|<span data-ttu-id="ee3ba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee3ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee3ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee3ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee3ba-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee3ba-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ee3ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee3ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee3ba-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee3ba-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ee3ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee3ba-115">Application</span></span>|<span data-ttu-id="ee3ba-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ee3ba-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee3ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee3ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee3ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee3ba-118">Optional query parameters</span></span>
<span data-ttu-id="ee3ba-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee3ba-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee3ba-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee3ba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3ba-121">Request headers</span></span>
|<span data-ttu-id="ee3ba-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ee3ba-122">Name</span></span>|<span data-ttu-id="ee3ba-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee3ba-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee3ba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee3ba-124">Authorization</span></span>|<span data-ttu-id="ee3ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee3ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3ba-127">Request body</span></span>
<span data-ttu-id="ee3ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee3ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee3ba-129">Response</span></span>

<span data-ttu-id="ee3ba-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee3ba-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee3ba-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee3ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3ba-132">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```


### <a name="response"></a><span data-ttu-id="ee3ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee3ba-133">Response</span></span>
<span data-ttu-id="ee3ba-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee3ba-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": [
    {
            "@odata.etag": "W/\"xzyPKP0BiUGgld+lMKXwbQAAgdhkVw==\"",
            "importance": "low",
            "isReminderOn": false,
            "status": "notStarted",
            "title": "Linked entity new task 1",
            "createdDateTime": "2020-07-08T11:15:19.9359889Z",
            "lastModifiedDateTime": "2020-07-08T11:15:20.0614375Z",
            "id": "AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD",
            "body": {
                "content": "",
                "contentType": "text"
            },
            "linkedResources@odata.context": "https://graph.microsoft.com/beta/$metadata#users('todoservicetest2412201901%40outlook.com')/todo/lists('35e2-35e2-721a-e235-1a72e2351a7')/tasks('AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD')/linkedResources",
            "linkedResources": [
                {
                    "applicationName": "Partner App Name",
                    "displayName": "Partner App Name",
                    "externalId": "teset1243434",
                    "id": "30911960-7321-4cba-9ba0-cdb68e2984c7"
                }
            ]
        }
  ]
}
```
