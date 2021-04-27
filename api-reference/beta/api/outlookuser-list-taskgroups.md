---
title: Listar taskGroups
description: Obter todos os Outlook de tarefas na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0d79ec13b68e68ab11180db9a0826a12b79a61b3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052968"
---
# <a name="list-taskgroups-deprecated"></a><span data-ttu-id="59185-103">Listar taskGroups (preterido)</span><span class="sxs-lookup"><span data-stu-id="59185-103">List taskGroups (deprecated)</span></span>

<span data-ttu-id="59185-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59185-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="59185-105">Obter todos os Outlook de tarefas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="59185-105">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="59185-106">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="59185-106">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="59185-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="59185-107">Permissions</span></span>
<span data-ttu-id="59185-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59185-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59185-110">Permission type</span></span>      | <span data-ttu-id="59185-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59185-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59185-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59185-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59185-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="59185-113">Tasks.Read</span></span>    |
|<span data-ttu-id="59185-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59185-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59185-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="59185-115">Tasks.Read</span></span>    |
|<span data-ttu-id="59185-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59185-116">Application</span></span> | <span data-ttu-id="59185-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59185-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59185-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59185-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59185-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59185-119">Optional query parameters</span></span>
<span data-ttu-id="59185-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59185-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59185-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59185-121">Request headers</span></span>
| <span data-ttu-id="59185-122">Nome</span><span class="sxs-lookup"><span data-stu-id="59185-122">Name</span></span>      |<span data-ttu-id="59185-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="59185-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59185-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="59185-124">Authorization</span></span>  | <span data-ttu-id="59185-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59185-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59185-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59185-127">Request body</span></span>
<span data-ttu-id="59185-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59185-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59185-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="59185-129">Response</span></span>

<span data-ttu-id="59185-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59185-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59185-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59185-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59185-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59185-132">Request</span></span>
<span data-ttu-id="59185-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59185-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59185-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59185-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="c"></a>[<span data-ttu-id="59185-135">C#</span><span class="sxs-lookup"><span data-stu-id="59185-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59185-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59185-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59185-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59185-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59185-138">Java</span><span class="sxs-lookup"><span data-stu-id="59185-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59185-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="59185-139">Response</span></span>
<span data-ttu-id="59185-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59185-140">Here is an example of the response.</span></span> <span data-ttu-id="59185-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59185-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
