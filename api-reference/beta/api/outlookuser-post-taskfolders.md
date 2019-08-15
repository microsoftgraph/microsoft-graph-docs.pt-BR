---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7463a6b96a6bac002b5a6c96cfb8b09857f0c0fc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413899"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="01eef-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="01eef-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01eef-104">Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="01eef-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="01eef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="01eef-105">Permissions</span></span>
<span data-ttu-id="01eef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01eef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01eef-108">Permission type</span></span>      | <span data-ttu-id="01eef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01eef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01eef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01eef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01eef-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01eef-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="01eef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01eef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01eef-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01eef-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="01eef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01eef-114">Application</span></span> | <span data-ttu-id="01eef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01eef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01eef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01eef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="01eef-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01eef-117">Request headers</span></span>
| <span data-ttu-id="01eef-118">Nome</span><span class="sxs-lookup"><span data-stu-id="01eef-118">Name</span></span>       | <span data-ttu-id="01eef-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="01eef-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01eef-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="01eef-120">Authorization</span></span>  | <span data-ttu-id="01eef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01eef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01eef-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01eef-123">Request body</span></span>
<span data-ttu-id="01eef-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="01eef-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="01eef-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="01eef-125">Response</span></span>

<span data-ttu-id="01eef-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01eef-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01eef-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01eef-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01eef-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01eef-128">Request</span></span>
<span data-ttu-id="01eef-129">O exemplo a seguir cria uma pasta de tarefas chamada voluntário no grupo de tarefas`My Tasks`padrão () da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="01eef-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01eef-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="01eef-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="01eef-131">C#</span><span class="sxs-lookup"><span data-stu-id="01eef-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01eef-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01eef-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01eef-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="01eef-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="01eef-134">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="01eef-134">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="01eef-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="01eef-135">Response</span></span>
<span data-ttu-id="01eef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01eef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
