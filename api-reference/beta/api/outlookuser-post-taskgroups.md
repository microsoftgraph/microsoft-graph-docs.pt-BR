---
title: Criar outlookTaskGroup
description: Criar um grupo de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ed70266ccd093128fa3d3f48c8999f7b615a759c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456182"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="0addd-103">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0addd-103">Create outlookTaskGroup</span></span>

<span data-ttu-id="0addd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0addd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0addd-105">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0addd-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="0addd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0addd-106">Permissions</span></span>
<span data-ttu-id="0addd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0addd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0addd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0addd-109">Permission type</span></span>      | <span data-ttu-id="0addd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0addd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0addd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0addd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0addd-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0addd-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0addd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0addd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0addd-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0addd-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0addd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0addd-115">Application</span></span> | <span data-ttu-id="0addd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0addd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0addd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0addd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="0addd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0addd-118">Request headers</span></span>
| <span data-ttu-id="0addd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0addd-119">Name</span></span>       | <span data-ttu-id="0addd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0addd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0addd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0addd-121">Authorization</span></span>  | <span data-ttu-id="0addd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0addd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0addd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0addd-124">Request body</span></span>
<span data-ttu-id="0addd-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0addd-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0addd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0addd-126">Response</span></span>

<span data-ttu-id="0addd-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0addd-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0addd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0addd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0addd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0addd-129">Request</span></span>
<span data-ttu-id="0addd-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0addd-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0addd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0addd-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0addd-132">C#</span><span class="sxs-lookup"><span data-stu-id="0addd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0addd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0addd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0addd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0addd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0addd-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0addd-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0addd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0addd-136">Response</span></span>
<span data-ttu-id="0addd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0addd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
