---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4250073177a5b5f0a77aa5f6957ad814ce017dfa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450783"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="347dd-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="347dd-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="347dd-104">Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="347dd-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="347dd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="347dd-105">Permissions</span></span>
<span data-ttu-id="347dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="347dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="347dd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="347dd-108">Permission type</span></span>      | <span data-ttu-id="347dd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="347dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="347dd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="347dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="347dd-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="347dd-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="347dd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="347dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="347dd-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="347dd-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="347dd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="347dd-114">Application</span></span> | <span data-ttu-id="347dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="347dd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="347dd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="347dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="347dd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="347dd-117">Request headers</span></span>
| <span data-ttu-id="347dd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="347dd-118">Name</span></span>       | <span data-ttu-id="347dd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="347dd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="347dd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="347dd-120">Authorization</span></span>  | <span data-ttu-id="347dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="347dd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="347dd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="347dd-123">Request body</span></span>
<span data-ttu-id="347dd-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="347dd-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="347dd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="347dd-125">Response</span></span>

<span data-ttu-id="347dd-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="347dd-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="347dd-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="347dd-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="347dd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="347dd-128">Request</span></span>
<span data-ttu-id="347dd-129">O exemplo a seguir cria uma pasta de tarefas chamada voluntário no grupo de tarefas`My Tasks`padrão () da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="347dd-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="347dd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="347dd-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="347dd-131">C#</span><span class="sxs-lookup"><span data-stu-id="347dd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="347dd-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="347dd-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="347dd-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="347dd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="347dd-134">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="347dd-134">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="347dd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="347dd-135">Response</span></span>
<span data-ttu-id="347dd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="347dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
