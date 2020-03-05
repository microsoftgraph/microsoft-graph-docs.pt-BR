---
title: Criar outlookTaskFolder
description: Criar uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d2a502f8675d752152c036d020b6999a5de887b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456100"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="1ea73-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1ea73-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="1ea73-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1ea73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ea73-105">Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ea73-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1ea73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ea73-106">Permissions</span></span>
<span data-ttu-id="1ea73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ea73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ea73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ea73-109">Permission type</span></span>      | <span data-ttu-id="1ea73-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ea73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ea73-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ea73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ea73-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ea73-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1ea73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ea73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ea73-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ea73-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1ea73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ea73-115">Application</span></span> | <span data-ttu-id="1ea73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ea73-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ea73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ea73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="1ea73-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea73-118">Request headers</span></span>
| <span data-ttu-id="1ea73-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1ea73-119">Name</span></span>       | <span data-ttu-id="1ea73-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea73-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ea73-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ea73-121">Authorization</span></span>  | <span data-ttu-id="1ea73-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ea73-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ea73-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea73-124">Request body</span></span>
<span data-ttu-id="1ea73-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="1ea73-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ea73-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea73-126">Response</span></span>

<span data-ttu-id="1ea73-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ea73-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ea73-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ea73-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ea73-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ea73-129">Request</span></span>
<span data-ttu-id="1ea73-130">O exemplo a seguir cria uma pasta de `Cooking` tarefas chamada no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="1ea73-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ea73-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ea73-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1ea73-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ea73-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1ea73-133">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="1ea73-133">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ea73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ea73-134">Response</span></span>
<span data-ttu-id="1ea73-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ea73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
