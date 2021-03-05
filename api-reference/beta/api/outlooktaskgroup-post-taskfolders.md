---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 285178adb4f0df591e1d1270d60b572f346d57e1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472892"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="eec02-103">Criar outlookTaskFolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="eec02-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="eec02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="eec02-105">Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup especificado.](../resources/outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="eec02-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="eec02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eec02-106">Permissions</span></span>
<span data-ttu-id="eec02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eec02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eec02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eec02-109">Permission type</span></span>      | <span data-ttu-id="eec02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eec02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eec02-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eec02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eec02-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec02-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="eec02-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eec02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec02-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eec02-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="eec02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eec02-115">Application</span></span> | <span data-ttu-id="eec02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eec02-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eec02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eec02-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="eec02-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eec02-118">Request headers</span></span>
| <span data-ttu-id="eec02-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eec02-119">Name</span></span>       | <span data-ttu-id="eec02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eec02-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eec02-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eec02-121">Authorization</span></span>  | <span data-ttu-id="eec02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eec02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eec02-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eec02-124">Request body</span></span>
<span data-ttu-id="eec02-125">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="eec02-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eec02-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eec02-126">Response</span></span>

<span data-ttu-id="eec02-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eec02-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eec02-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eec02-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eec02-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eec02-129">Request</span></span>
<span data-ttu-id="eec02-130">O exemplo a seguir cria uma pasta de tarefas `Cooking` chamada no grupo de tarefas especificado.</span><span class="sxs-lookup"><span data-stu-id="eec02-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

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

<span data-ttu-id="eec02-131">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="eec02-131">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eec02-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eec02-132">Response</span></span>
<span data-ttu-id="eec02-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eec02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


