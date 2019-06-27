---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 696080a7e35884839f7205cf3b137b1123613c15
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269157"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="9b9b8-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9b9b8-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b9b8-104">Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b9b8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b9b8-105">Permissions</span></span>
<span data-ttu-id="9b9b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9b8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b9b8-108">Permission type</span></span>      | <span data-ttu-id="9b9b8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b9b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b9b8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b9b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b9b8-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b9b8-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9b9b8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b9b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b9b8-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b9b8-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9b9b8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b9b8-114">Application</span></span> | <span data-ttu-id="9b9b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b9b8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b9b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="9b9b8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9b8-117">Request headers</span></span>
| <span data-ttu-id="9b9b8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b9b8-118">Name</span></span>       | <span data-ttu-id="9b9b8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b9b8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b9b8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b9b8-120">Authorization</span></span>  | <span data-ttu-id="9b9b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b9b8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9b8-123">Request body</span></span>
<span data-ttu-id="9b9b8-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="9b9b8-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9b9b8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b9b8-125">Response</span></span>

<span data-ttu-id="9b9b8-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b9b8-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b9b8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b9b8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9b8-128">Request</span></span>
<span data-ttu-id="9b9b8-129">O exemplo a seguir cria uma pasta de tarefas chamada voluntário no grupo de tarefas`My Tasks`padrão () da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="9b9b8-130">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="9b9b8-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9b9b8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b9b8-131">Response</span></span>
<span data-ttu-id="9b9b8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b9b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b9b8-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9b9b8-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b9b8-136">C#</span><span class="sxs-lookup"><span data-stu-id="9b9b8-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktaskfolder_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b9b8-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b9b8-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktaskfolder_from_outlookuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9b9b8-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9b9b8-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_outlooktaskfolder_from_outlookuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
