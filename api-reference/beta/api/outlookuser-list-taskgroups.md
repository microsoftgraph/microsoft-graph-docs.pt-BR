---
title: Listar taskGroups
description: Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8be733eb736b8288818ed3e5e8631dc7fd998cea
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461554"
---
# <a name="list-taskgroups-deprecated"></a><span data-ttu-id="c257c-103">Listar taskGroups (preterido)</span><span class="sxs-lookup"><span data-stu-id="c257c-103">List taskGroups (deprecated)</span></span>

<span data-ttu-id="c257c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c257c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="c257c-105">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c257c-105">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="c257c-106">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c257c-106">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="c257c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c257c-107">Permissions</span></span>
<span data-ttu-id="c257c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c257c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c257c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c257c-110">Permission type</span></span>      | <span data-ttu-id="c257c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c257c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c257c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c257c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c257c-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c257c-113">Tasks.Read</span></span>    |
|<span data-ttu-id="c257c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c257c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c257c-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c257c-115">Tasks.Read</span></span>    |
|<span data-ttu-id="c257c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c257c-116">Application</span></span> | <span data-ttu-id="c257c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c257c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c257c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c257c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c257c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c257c-119">Optional query parameters</span></span>
<span data-ttu-id="c257c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c257c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c257c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c257c-121">Request headers</span></span>
| <span data-ttu-id="c257c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c257c-122">Name</span></span>      |<span data-ttu-id="c257c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c257c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c257c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c257c-124">Authorization</span></span>  | <span data-ttu-id="c257c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c257c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c257c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c257c-127">Request body</span></span>
<span data-ttu-id="c257c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c257c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c257c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c257c-129">Response</span></span>

<span data-ttu-id="c257c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c257c-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c257c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c257c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c257c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c257c-132">Request</span></span>
<span data-ttu-id="c257c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c257c-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c257c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c257c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="c"></a>[<span data-ttu-id="c257c-135">C#</span><span class="sxs-lookup"><span data-stu-id="c257c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c257c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c257c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c257c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c257c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c257c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c257c-138">Response</span></span>
<span data-ttu-id="c257c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c257c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
