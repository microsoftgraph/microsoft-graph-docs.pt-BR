---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9aafda49a7d02169c791c4038195aca4d387928b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038002"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="046ee-103">Criar outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="046ee-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="046ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="046ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="046ee-105">Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="046ee-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="046ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="046ee-106">Permissions</span></span>
<span data-ttu-id="046ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="046ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="046ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="046ee-109">Permission type</span></span>      | <span data-ttu-id="046ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="046ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="046ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="046ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="046ee-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="046ee-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="046ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="046ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="046ee-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="046ee-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="046ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="046ee-115">Application</span></span> | <span data-ttu-id="046ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="046ee-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="046ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="046ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="046ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="046ee-118">Request headers</span></span>
| <span data-ttu-id="046ee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="046ee-119">Name</span></span>       | <span data-ttu-id="046ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="046ee-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="046ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="046ee-121">Authorization</span></span>  | <span data-ttu-id="046ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="046ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="046ee-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="046ee-124">Request body</span></span>
<span data-ttu-id="046ee-125">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="046ee-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="046ee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="046ee-126">Response</span></span>

<span data-ttu-id="046ee-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="046ee-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="046ee-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="046ee-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="046ee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="046ee-129">Request</span></span>
<span data-ttu-id="046ee-130">O exemplo a seguir cria uma pasta de tarefas chamada Voluntário no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="046ee-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="046ee-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="046ee-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="046ee-132">C#</span><span class="sxs-lookup"><span data-stu-id="046ee-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="046ee-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="046ee-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="046ee-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="046ee-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="046ee-135">Java</span><span class="sxs-lookup"><span data-stu-id="046ee-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="046ee-136">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="046ee-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="046ee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="046ee-137">Response</span></span>
<span data-ttu-id="046ee-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="046ee-138">Here is an example of the response.</span></span> <span data-ttu-id="046ee-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="046ee-139">Note: The response object shown here might be shortened for readability.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
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
  "suppressions": [
  ]
}
-->


