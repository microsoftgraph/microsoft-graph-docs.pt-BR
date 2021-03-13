---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ae45fb686c3b76156b0423ee3890fd306502aa82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774247"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="df6ca-103">Criar outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="df6ca-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="df6ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df6ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="df6ca-105">Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup especificado.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="df6ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df6ca-106">Permissions</span></span>
<span data-ttu-id="df6ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df6ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df6ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df6ca-109">Permission type</span></span>      | <span data-ttu-id="df6ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df6ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df6ca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df6ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df6ca-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df6ca-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="df6ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df6ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df6ca-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df6ca-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="df6ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df6ca-115">Application</span></span> | <span data-ttu-id="df6ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df6ca-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df6ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df6ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="df6ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df6ca-118">Request headers</span></span>
| <span data-ttu-id="df6ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="df6ca-119">Name</span></span>       | <span data-ttu-id="df6ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="df6ca-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df6ca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="df6ca-121">Authorization</span></span>  | <span data-ttu-id="df6ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df6ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df6ca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df6ca-124">Request body</span></span>
<span data-ttu-id="df6ca-125">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df6ca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="df6ca-126">Response</span></span>

<span data-ttu-id="df6ca-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df6ca-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df6ca-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df6ca-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df6ca-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df6ca-129">Request</span></span>
<span data-ttu-id="df6ca-130">O exemplo a seguir cria uma pasta de tarefas `Cooking` chamada no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="df6ca-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>


# <a name="http"></a>[<span data-ttu-id="df6ca-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="df6ca-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
# <a name="c"></a>[<span data-ttu-id="df6ca-132">C#</span><span class="sxs-lookup"><span data-stu-id="df6ca-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df6ca-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df6ca-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df6ca-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df6ca-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df6ca-135">Java</span><span class="sxs-lookup"><span data-stu-id="df6ca-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="df6ca-136">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="df6ca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="df6ca-137">Response</span></span>
<span data-ttu-id="df6ca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df6ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


