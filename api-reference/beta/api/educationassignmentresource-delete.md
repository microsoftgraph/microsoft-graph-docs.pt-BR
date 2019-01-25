---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0a6ac6f4cddde9d80e48080b0f54b2610e84782c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513036"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="27bb1-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="27bb1-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27bb1-104">Exclua um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="27bb1-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="27bb1-105">Somente professores na classe podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="27bb1-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="27bb1-106">Depois que uma atribuição tiver sido publicada aos alunos, professores não é possível remover os recursos que são marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="27bb1-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="27bb1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27bb1-107">Permissions</span></span>
<span data-ttu-id="27bb1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27bb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27bb1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27bb1-110">Permission type</span></span>      | <span data-ttu-id="27bb1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27bb1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27bb1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27bb1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="27bb1-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27bb1-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="27bb1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27bb1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="27bb1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27bb1-115">Not supported.</span></span>  |
|<span data-ttu-id="27bb1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27bb1-116">Application</span></span> | <span data-ttu-id="27bb1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27bb1-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="27bb1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27bb1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="27bb1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27bb1-119">Request headers</span></span>
| <span data-ttu-id="27bb1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27bb1-120">Header</span></span>       | <span data-ttu-id="27bb1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27bb1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27bb1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27bb1-122">Authorization</span></span>  | <span data-ttu-id="27bb1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27bb1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27bb1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27bb1-125">Request body</span></span>
<span data-ttu-id="27bb1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27bb1-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="27bb1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bb1-127">Response</span></span>
<span data-ttu-id="27bb1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27bb1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27bb1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27bb1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27bb1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27bb1-131">Request</span></span>
<span data-ttu-id="27bb1-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27bb1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="27bb1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bb1-133">Response</span></span>
<span data-ttu-id="27bb1-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27bb1-134">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
