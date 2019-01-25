---
title: Criar outlookTaskGroup
description: Crie um grupo de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 291eb580228f28754acccff78f60ed6a2004155b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516004"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="6ee16-103">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="6ee16-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee16-104">Crie um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6ee16-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ee16-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ee16-105">Permissions</span></span>
<span data-ttu-id="6ee16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee16-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ee16-108">Permission type</span></span>      | <span data-ttu-id="6ee16-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ee16-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ee16-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ee16-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ee16-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ee16-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6ee16-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ee16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee16-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ee16-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6ee16-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ee16-114">Application</span></span> | <span data-ttu-id="6ee16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ee16-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ee16-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="6ee16-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee16-117">Request headers</span></span>
| <span data-ttu-id="6ee16-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6ee16-118">Name</span></span>       | <span data-ttu-id="6ee16-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee16-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ee16-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ee16-120">Authorization</span></span>  | <span data-ttu-id="6ee16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ee16-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee16-123">Request body</span></span>
<span data-ttu-id="6ee16-124">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6ee16-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ee16-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee16-125">Response</span></span>

<span data-ttu-id="6ee16-126">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ee16-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ee16-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ee16-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ee16-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee16-128">Request</span></span>
<span data-ttu-id="6ee16-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ee16-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="6ee16-130">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6ee16-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6ee16-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee16-131">Response</span></span>
<span data-ttu-id="6ee16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ee16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
