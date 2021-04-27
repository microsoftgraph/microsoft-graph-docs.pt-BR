---
title: Criar outlookTaskGroup
description: Crie um Outlook de tarefas na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1cef21d441ba20c1bc97f7e4bf2e4f1c922d1f9c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037995"
---
# <a name="create-outlooktaskgroup-deprecated"></a><span data-ttu-id="1ef91-103">Criar outlookTaskGroup (preterido)</span><span class="sxs-lookup"><span data-stu-id="1ef91-103">Create outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="1ef91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="1ef91-105">Crie um Outlook de tarefas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="1ef91-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ef91-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ef91-106">Permissions</span></span>
<span data-ttu-id="1ef91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ef91-109">Permission type</span></span>      | <span data-ttu-id="1ef91-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ef91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ef91-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ef91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ef91-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ef91-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1ef91-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ef91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef91-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ef91-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1ef91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ef91-115">Application</span></span> | <span data-ttu-id="1ef91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ef91-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="1ef91-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef91-118">Request headers</span></span>
| <span data-ttu-id="1ef91-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1ef91-119">Name</span></span>       | <span data-ttu-id="1ef91-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef91-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ef91-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ef91-121">Authorization</span></span>  | <span data-ttu-id="1ef91-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ef91-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef91-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef91-124">Request body</span></span>
<span data-ttu-id="1ef91-125">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskGroup.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1ef91-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ef91-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef91-126">Response</span></span>

<span data-ttu-id="1ef91-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ef91-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef91-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ef91-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ef91-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ef91-129">Request</span></span>
<span data-ttu-id="1ef91-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ef91-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ef91-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ef91-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
# <a name="c"></a>[<span data-ttu-id="1ef91-132">C#</span><span class="sxs-lookup"><span data-stu-id="1ef91-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ef91-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ef91-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ef91-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ef91-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ef91-135">Java</span><span class="sxs-lookup"><span data-stu-id="1ef91-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskgroup-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1ef91-136">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskGroup.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1ef91-136">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ef91-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ef91-137">Response</span></span>
<span data-ttu-id="1ef91-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ef91-138">Here is an example of the response.</span></span> <span data-ttu-id="1ef91-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1ef91-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


