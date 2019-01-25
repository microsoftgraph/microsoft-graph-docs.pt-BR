---
title: Excluir educationAssignment
description: Exclua uma atribuição existente. Somente professores dentro de uma classe podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2356330a75558ea88b94c9266fb2d4a387e87b59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515885"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="44ed8-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="44ed8-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44ed8-105">Exclua uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="44ed8-105">Delete an existing assignment.</span></span> <span data-ttu-id="44ed8-106">Somente professores dentro de uma classe podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="44ed8-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="44ed8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="44ed8-107">Permissions</span></span>
<span data-ttu-id="44ed8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ed8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ed8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44ed8-110">Permission type</span></span>      | <span data-ttu-id="44ed8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44ed8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44ed8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44ed8-112">Delegated (work or school account)</span></span>| <span data-ttu-id="44ed8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44ed8-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="44ed8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44ed8-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="44ed8-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="44ed8-115">Not Supported.</span></span> |
|<span data-ttu-id="44ed8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44ed8-116">Application</span></span> | <span data-ttu-id="44ed8-117">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="44ed8-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="44ed8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44ed8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="44ed8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44ed8-119">Request headers</span></span>
| <span data-ttu-id="44ed8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44ed8-120">Header</span></span>       | <span data-ttu-id="44ed8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44ed8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44ed8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44ed8-122">Authorization</span></span>  | <span data-ttu-id="44ed8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44ed8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44ed8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44ed8-125">Request body</span></span>
<span data-ttu-id="44ed8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44ed8-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="44ed8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ed8-127">Response</span></span>
<span data-ttu-id="44ed8-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44ed8-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ed8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44ed8-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="44ed8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44ed8-131">Request</span></span>
<span data-ttu-id="44ed8-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44ed8-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="44ed8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="44ed8-133">Response</span></span>
<span data-ttu-id="44ed8-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44ed8-134">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
