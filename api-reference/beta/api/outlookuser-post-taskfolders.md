---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7f1c1767f125da2745837addb7852805630f5231
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849314"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="03dd0-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="03dd0-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="03dd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03dd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="03dd0-105">Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="03dd0-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="03dd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03dd0-106">Permissions</span></span>
<span data-ttu-id="03dd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03dd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03dd0-109">Permission type</span></span>      | <span data-ttu-id="03dd0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03dd0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03dd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03dd0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03dd0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03dd0-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="03dd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03dd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03dd0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03dd0-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="03dd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03dd0-115">Application</span></span> | <span data-ttu-id="03dd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03dd0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03dd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03dd0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="03dd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03dd0-118">Request headers</span></span>
| <span data-ttu-id="03dd0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="03dd0-119">Name</span></span>       | <span data-ttu-id="03dd0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="03dd0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03dd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="03dd0-121">Authorization</span></span>  | <span data-ttu-id="03dd0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03dd0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03dd0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03dd0-124">Request body</span></span>
<span data-ttu-id="03dd0-125">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="03dd0-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03dd0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="03dd0-126">Response</span></span>

<span data-ttu-id="03dd0-127">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03dd0-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03dd0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03dd0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03dd0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03dd0-129">Request</span></span>
<span data-ttu-id="03dd0-130">O exemplo a seguir cria uma pasta de tarefas chamada voluntário no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="03dd0-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="03dd0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="03dd0-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03dd0-132">C#</span><span class="sxs-lookup"><span data-stu-id="03dd0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03dd0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03dd0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03dd0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03dd0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="03dd0-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="03dd0-135">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03dd0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="03dd0-136">Response</span></span>
<span data-ttu-id="03dd0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03dd0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
