---
title: Criar outlookTaskGroup
description: Criar um grupo de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 364510c3d866b193012763d17dbc22f2e1d7c8f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539656"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="f29bb-103">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f29bb-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f29bb-104">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f29bb-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="f29bb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f29bb-105">Permissions</span></span>
<span data-ttu-id="f29bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29bb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f29bb-108">Permission type</span></span>      | <span data-ttu-id="f29bb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f29bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f29bb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f29bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f29bb-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29bb-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f29bb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f29bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f29bb-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29bb-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f29bb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f29bb-114">Application</span></span> | <span data-ttu-id="f29bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f29bb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f29bb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f29bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="f29bb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f29bb-117">Request headers</span></span>
| <span data-ttu-id="f29bb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f29bb-118">Name</span></span>       | <span data-ttu-id="f29bb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f29bb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f29bb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f29bb-120">Authorization</span></span>  | <span data-ttu-id="f29bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f29bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f29bb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f29bb-123">Request body</span></span>
<span data-ttu-id="f29bb-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="f29bb-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f29bb-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29bb-125">Response</span></span>

<span data-ttu-id="f29bb-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f29bb-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29bb-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f29bb-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f29bb-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f29bb-128">Request</span></span>
<span data-ttu-id="f29bb-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f29bb-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="f29bb-130">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="f29bb-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f29bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f29bb-131">Response</span></span>
<span data-ttu-id="f29bb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f29bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
