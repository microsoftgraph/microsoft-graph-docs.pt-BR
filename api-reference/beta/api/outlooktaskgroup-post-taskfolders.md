---
title: Criar outlookTaskFolder
description: Criar uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 328f250b3f3116576734ac4218959576c0930914
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633668"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="57960-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="57960-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57960-104">Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="57960-104">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="57960-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="57960-105">Permissions</span></span>
<span data-ttu-id="57960-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57960-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57960-108">Permission type</span></span>      | <span data-ttu-id="57960-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57960-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57960-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57960-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57960-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57960-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="57960-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57960-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57960-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57960-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="57960-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57960-114">Application</span></span> | <span data-ttu-id="57960-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57960-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57960-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57960-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="57960-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57960-117">Request headers</span></span>
| <span data-ttu-id="57960-118">Nome</span><span class="sxs-lookup"><span data-stu-id="57960-118">Name</span></span>       | <span data-ttu-id="57960-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="57960-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57960-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="57960-120">Authorization</span></span>  | <span data-ttu-id="57960-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57960-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57960-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57960-123">Request body</span></span>
<span data-ttu-id="57960-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="57960-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57960-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="57960-125">Response</span></span>

<span data-ttu-id="57960-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57960-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57960-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57960-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57960-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57960-128">Request</span></span>
<span data-ttu-id="57960-129">O exemplo a seguir cria uma pasta de `Cooking` tarefas chamada no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="57960-129">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57960-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="57960-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups/AAMkADIyAAAhrbe-AAA'/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57960-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57960-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="57960-132">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="57960-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="57960-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="57960-133">Response</span></span>
<span data-ttu-id="57960-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57960-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
