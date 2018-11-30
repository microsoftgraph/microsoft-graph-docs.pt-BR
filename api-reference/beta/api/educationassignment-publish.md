---
title: 'educationAssignment: publicar'
description: Esta ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado. Somente um professor na classe pode fazer essa chamada. Quando uma atribuição está no status de rascunho, alunos não verá a atribuição, nem haverá quaisquer objetos de envio. Quando você chamar essa API, são criados objetos de envio e a atribuição aparece na lista de student.
ms.openlocfilehash: d5de5a45d437662dbcd2bf869aef93502a3669f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033993"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="e31f0-106">educationAssignment: publicar</span><span class="sxs-lookup"><span data-stu-id="e31f0-106">educationAssignment: publish</span></span>

> <span data-ttu-id="e31f0-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e31f0-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e31f0-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e31f0-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e31f0-109">Esta ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado.</span><span class="sxs-lookup"><span data-stu-id="e31f0-109">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="e31f0-110">Somente um professor na classe pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="e31f0-110">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="e31f0-111">Quando uma atribuição está no status de rascunho, alunos não verá a atribuição, nem haverá quaisquer objetos de envio.</span><span class="sxs-lookup"><span data-stu-id="e31f0-111">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="e31f0-112">Quando você chamar essa API, são criados objetos de envio e a atribuição aparece na lista de student.</span><span class="sxs-lookup"><span data-stu-id="e31f0-112">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e31f0-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="e31f0-113">Permissions</span></span>
<span data-ttu-id="e31f0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31f0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e31f0-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e31f0-116">Permission type</span></span>      | <span data-ttu-id="e31f0-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e31f0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e31f0-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e31f0-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="e31f0-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e31f0-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e31f0-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e31f0-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e31f0-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e31f0-121">Not supported.</span></span>  |
|<span data-ttu-id="e31f0-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e31f0-122">Application</span></span> | <span data-ttu-id="e31f0-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e31f0-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e31f0-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e31f0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="e31f0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e31f0-125">Request headers</span></span>
| <span data-ttu-id="e31f0-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e31f0-126">Header</span></span>       | <span data-ttu-id="e31f0-127">Valor</span><span class="sxs-lookup"><span data-stu-id="e31f0-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e31f0-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e31f0-128">Authorization</span></span>  | <span data-ttu-id="e31f0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e31f0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e31f0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e31f0-131">Request body</span></span>
<span data-ttu-id="e31f0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e31f0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e31f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31f0-133">Response</span></span>
<span data-ttu-id="e31f0-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e31f0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31f0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e31f0-136">Example</span></span>
<span data-ttu-id="e31f0-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e31f0-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e31f0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e31f0-138">Request</span></span>
<span data-ttu-id="e31f0-139">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e31f0-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="e31f0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e31f0-140">Response</span></span>
<span data-ttu-id="e31f0-141">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e31f0-141">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
