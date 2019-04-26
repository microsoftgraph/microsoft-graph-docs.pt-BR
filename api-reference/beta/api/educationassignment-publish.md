---
title: 'educationAssignment: publish'
description: Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado. Apenas um professor na turma pode fazer essa chamada. Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio. Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: f6b13329529c35230276783a3e824f0a53e3ca17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325118"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="3a614-106">educationAssignment: publish</span><span class="sxs-lookup"><span data-stu-id="3a614-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a614-107">Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado.</span><span class="sxs-lookup"><span data-stu-id="3a614-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="3a614-108">Apenas um professor na turma pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="3a614-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="3a614-109">Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="3a614-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="3a614-110">Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.</span><span class="sxs-lookup"><span data-stu-id="3a614-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a614-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a614-111">Permissions</span></span>
<span data-ttu-id="3a614-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a614-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a614-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a614-114">Permission type</span></span>      | <span data-ttu-id="3a614-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a614-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a614-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a614-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a614-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a614-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3a614-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a614-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3a614-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a614-119">Not supported.</span></span>  |
|<span data-ttu-id="3a614-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a614-120">Application</span></span> | <span data-ttu-id="3a614-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a614-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a614-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a614-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="3a614-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a614-123">Request headers</span></span>
| <span data-ttu-id="3a614-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a614-124">Header</span></span>       | <span data-ttu-id="3a614-125">Valor</span><span class="sxs-lookup"><span data-stu-id="3a614-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a614-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a614-126">Authorization</span></span>  | <span data-ttu-id="3a614-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a614-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a614-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a614-129">Request body</span></span>
<span data-ttu-id="3a614-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a614-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a614-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a614-131">Response</span></span>
<span data-ttu-id="3a614-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a614-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a614-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a614-134">Example</span></span>
<span data-ttu-id="3a614-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3a614-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a614-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a614-136">Request</span></span>
<span data-ttu-id="3a614-137">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a614-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="3a614-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a614-138">Response</span></span>
<span data-ttu-id="3a614-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3a614-139">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
