---
title: Excluir outlookTaskFolder
description: Excluir a pasta de tarefas do Outlook especificada.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8e5517f61327ff26e9e84fdb93faf5be40e1a1d3
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849697"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="c5695-103">Excluir outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c5695-103">Delete outlookTaskFolder</span></span>

<span data-ttu-id="c5695-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="c5695-105">Excluir a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="c5695-105">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5695-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5695-106">Permissions</span></span>
<span data-ttu-id="c5695-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5695-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5695-109">Permission type</span></span>      | <span data-ttu-id="c5695-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5695-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5695-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5695-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5695-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5695-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c5695-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5695-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5695-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5695-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c5695-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5695-115">Application</span></span> | <span data-ttu-id="c5695-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5695-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5695-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5695-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c5695-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5695-118">Request headers</span></span>
| <span data-ttu-id="c5695-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c5695-119">Name</span></span>       | <span data-ttu-id="c5695-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5695-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5695-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5695-121">Authorization</span></span>  | <span data-ttu-id="c5695-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5695-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5695-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5695-124">Request body</span></span>
<span data-ttu-id="c5695-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5695-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5695-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5695-126">Response</span></span>

<span data-ttu-id="c5695-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5695-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5695-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5695-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5695-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5695-130">Request</span></span>
<span data-ttu-id="c5695-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5695-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5695-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5695-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="c5695-133">C#</span><span class="sxs-lookup"><span data-stu-id="c5695-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5695-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5695-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5695-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5695-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5695-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5695-136">Response</span></span>
<span data-ttu-id="c5695-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5695-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
