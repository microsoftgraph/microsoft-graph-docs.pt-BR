---
title: Criar outlookTaskGroup
description: Criar um grupo de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 19a04ff22ff569dc0f277e3ff434143d3fce4ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456041"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="3f84d-103">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="3f84d-103">Create outlookTaskGroup</span></span>

<span data-ttu-id="3f84d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f84d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f84d-105">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f84d-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f84d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f84d-106">Permissions</span></span>
<span data-ttu-id="3f84d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f84d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f84d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f84d-109">Permission type</span></span>      | <span data-ttu-id="3f84d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f84d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f84d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f84d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f84d-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f84d-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3f84d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f84d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f84d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f84d-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3f84d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f84d-115">Application</span></span> | <span data-ttu-id="3f84d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f84d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f84d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f84d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="3f84d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84d-118">Request headers</span></span>
| <span data-ttu-id="3f84d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3f84d-119">Name</span></span>       | <span data-ttu-id="3f84d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f84d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3f84d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f84d-121">Authorization</span></span>  | <span data-ttu-id="3f84d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f84d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f84d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84d-124">Request body</span></span>
<span data-ttu-id="3f84d-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="3f84d-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f84d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f84d-126">Response</span></span>

<span data-ttu-id="3f84d-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f84d-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f84d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f84d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f84d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84d-129">Request</span></span>
<span data-ttu-id="3f84d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f84d-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f84d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f84d-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3f84d-132">C#</span><span class="sxs-lookup"><span data-stu-id="3f84d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f84d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f84d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f84d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f84d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3f84d-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="3f84d-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3f84d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f84d-136">Response</span></span>
<span data-ttu-id="3f84d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f84d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
