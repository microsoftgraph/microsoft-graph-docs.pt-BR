---
title: Excluir outlookTaskFolder
description: Excluir a pasta de tarefas do Outlook especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4c526c937f7d92b6e2b0482193f6c0327f4870c1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869383"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="7a474-103">Excluir outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7a474-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a474-104">Excluir a pasta de tarefas do Outlook especificada.</span><span class="sxs-lookup"><span data-stu-id="7a474-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a474-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a474-105">Permissions</span></span>
<span data-ttu-id="7a474-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a474-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a474-108">Permission type</span></span>      | <span data-ttu-id="7a474-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a474-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a474-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a474-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a474-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a474-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a474-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a474-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a474-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a474-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a474-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a474-114">Application</span></span> | <span data-ttu-id="7a474-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a474-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a474-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a474-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7a474-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a474-117">Request headers</span></span>
| <span data-ttu-id="7a474-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7a474-118">Name</span></span>       | <span data-ttu-id="7a474-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a474-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a474-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a474-120">Authorization</span></span>  | <span data-ttu-id="7a474-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a474-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a474-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a474-123">Request body</span></span>
<span data-ttu-id="7a474-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a474-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a474-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a474-125">Response</span></span>

<span data-ttu-id="7a474-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a474-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a474-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a474-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a474-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a474-129">Request</span></span>
<span data-ttu-id="7a474-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a474-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="7a474-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a474-131">Response</span></span>
<span data-ttu-id="7a474-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a474-132">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
