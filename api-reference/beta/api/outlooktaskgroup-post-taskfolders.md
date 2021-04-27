---
title: Criar outlookTaskFolder
description: Crie uma Outlook de tarefas em um outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e7fd36eae4980a533f4d3bc02223bab788f8e7a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049216"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="dac54-103">Criar outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="dac54-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="dac54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="dac54-105">Crie uma Outlook de tarefas em um [outlookTaskGroup especificado.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="dac54-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dac54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dac54-106">Permissions</span></span>
<span data-ttu-id="dac54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dac54-109">Permission type</span></span>      | <span data-ttu-id="dac54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dac54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dac54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dac54-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac54-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dac54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dac54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac54-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac54-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dac54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dac54-115">Application</span></span> | <span data-ttu-id="dac54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dac54-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac54-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dac54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="dac54-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dac54-118">Request headers</span></span>
| <span data-ttu-id="dac54-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dac54-119">Name</span></span>       | <span data-ttu-id="dac54-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac54-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dac54-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dac54-121">Authorization</span></span>  | <span data-ttu-id="dac54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dac54-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dac54-124">Request body</span></span>
<span data-ttu-id="dac54-125">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="dac54-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dac54-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac54-126">Response</span></span>

<span data-ttu-id="dac54-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac54-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac54-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dac54-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dac54-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac54-129">Request</span></span>
<span data-ttu-id="dac54-130">O exemplo a seguir cria uma pasta de tarefas `Cooking` chamada no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="dac54-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>


# <a name="http"></a>[<span data-ttu-id="dac54-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="dac54-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dac54-132">C#</span><span class="sxs-lookup"><span data-stu-id="dac54-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dac54-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dac54-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dac54-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dac54-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dac54-135">Java</span><span class="sxs-lookup"><span data-stu-id="dac54-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="dac54-136">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="dac54-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dac54-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac54-137">Response</span></span>
<span data-ttu-id="dac54-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac54-138">Here is an example of the response.</span></span> <span data-ttu-id="dac54-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dac54-139">Note: The response object shown here might be shortened for readability.</span></span>
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


