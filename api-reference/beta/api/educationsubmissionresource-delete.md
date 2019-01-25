---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a735cb1451e8d3eb8df13e6fa395c3e02393f451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518979"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="1df18-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="1df18-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df18-106">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="1df18-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="1df18-107">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="1df18-107">This can only be done by the student.</span></span> <span data-ttu-id="1df18-108">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada depois que a cópia atual for excluída.</span><span class="sxs-lookup"><span data-stu-id="1df18-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="1df18-109">Isso permite "Redefinir" o recurso ao seu estado original.</span><span class="sxs-lookup"><span data-stu-id="1df18-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="1df18-110">Se o recurso não foi copiado da atribuição, mas foi adicionado de student, o recurso simplesmente é excluído.</span><span class="sxs-lookup"><span data-stu-id="1df18-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="1df18-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1df18-111">Permissions</span></span>
<span data-ttu-id="1df18-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1df18-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1df18-114">Permission type</span></span>      | <span data-ttu-id="1df18-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1df18-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1df18-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1df18-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="1df18-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1df18-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1df18-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1df18-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1df18-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1df18-119">Not supported.</span></span>  |
|<span data-ttu-id="1df18-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1df18-120">Application</span></span> | <span data-ttu-id="1df18-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1df18-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1df18-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1df18-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1df18-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1df18-123">Request headers</span></span>
| <span data-ttu-id="1df18-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1df18-124">Header</span></span>       | <span data-ttu-id="1df18-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1df18-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1df18-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1df18-126">Authorization</span></span>  | <span data-ttu-id="1df18-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1df18-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1df18-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1df18-129">Request body</span></span>
<span data-ttu-id="1df18-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1df18-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1df18-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1df18-131">Response</span></span>
<span data-ttu-id="1df18-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1df18-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1df18-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1df18-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1df18-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1df18-135">Request</span></span>
<span data-ttu-id="1df18-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1df18-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="1df18-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1df18-137">Response</span></span>
<span data-ttu-id="1df18-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1df18-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
