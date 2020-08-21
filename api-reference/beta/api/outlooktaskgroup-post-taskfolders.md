---
title: Criar outlookTaskFolder
description: Criar uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a058c8289efc384416937d144ae35f6379214609
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849209"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="76fbb-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="76fbb-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="76fbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76fbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="76fbb-105">Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="76fbb-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="76fbb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="76fbb-106">Permissions</span></span>
<span data-ttu-id="76fbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76fbb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76fbb-109">Permission type</span></span>      | <span data-ttu-id="76fbb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76fbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76fbb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76fbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="76fbb-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76fbb-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="76fbb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76fbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76fbb-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76fbb-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="76fbb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76fbb-115">Application</span></span> | <span data-ttu-id="76fbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76fbb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76fbb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76fbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="76fbb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbb-118">Request headers</span></span>
| <span data-ttu-id="76fbb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="76fbb-119">Name</span></span>       | <span data-ttu-id="76fbb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76fbb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76fbb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="76fbb-121">Authorization</span></span>  | <span data-ttu-id="76fbb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76fbb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76fbb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbb-124">Request body</span></span>
<span data-ttu-id="76fbb-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="76fbb-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="76fbb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="76fbb-126">Response</span></span>

<span data-ttu-id="76fbb-127">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76fbb-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76fbb-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76fbb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76fbb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76fbb-129">Request</span></span>
<span data-ttu-id="76fbb-130">O exemplo a seguir cria uma pasta de tarefas chamada `Cooking` no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="76fbb-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

# <a name="http"></a>[<span data-ttu-id="76fbb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="76fbb-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="76fbb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76fbb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="76fbb-133">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="76fbb-133">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="76fbb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76fbb-134">Response</span></span>
<span data-ttu-id="76fbb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76fbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
