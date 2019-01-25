---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 81c77d96b4d7c66cfbc7dde3481a7bfaa8cd6c5f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514443"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="556c0-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="556c0-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="556c0-104">Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="556c0-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="556c0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="556c0-105">Permissions</span></span>
<span data-ttu-id="556c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="556c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="556c0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="556c0-108">Permission type</span></span>      | <span data-ttu-id="556c0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="556c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="556c0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="556c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="556c0-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="556c0-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="556c0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="556c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="556c0-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="556c0-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="556c0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="556c0-114">Application</span></span> | <span data-ttu-id="556c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="556c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="556c0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="556c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="556c0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="556c0-117">Request headers</span></span>
| <span data-ttu-id="556c0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="556c0-118">Name</span></span>       | <span data-ttu-id="556c0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="556c0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="556c0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="556c0-120">Authorization</span></span>  | <span data-ttu-id="556c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="556c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="556c0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="556c0-123">Request body</span></span>
<span data-ttu-id="556c0-124">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="556c0-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="556c0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="556c0-125">Response</span></span>

<span data-ttu-id="556c0-126">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="556c0-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="556c0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="556c0-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="556c0-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="556c0-128">Request</span></span>
<span data-ttu-id="556c0-129">O exemplo a seguir cria uma pasta de tarefas chamada dos alunos no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="556c0-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="556c0-130">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="556c0-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="556c0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="556c0-131">Response</span></span>
<span data-ttu-id="556c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="556c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
