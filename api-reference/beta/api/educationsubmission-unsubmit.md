---
title: 'educationSubmission: unsubmit'
description: . Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Balde workingResources. O professor será observando a lista de recursos úteis para a classificação.
ms.openlocfilehash: 610b5a69a06c29d2e2b9b1fa6eb501a56d59b076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034001"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="28f23-105">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="28f23-105">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="28f23-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28f23-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28f23-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28f23-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28f23-108">Uma ação que indica que um estudante deseja trabalhar no envio da atribuição depois que ele foi ativado.</span><span class="sxs-lookup"><span data-stu-id="28f23-108">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="28f23-109">Essa ação só pode ser executada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="28f23-109">This action can only be taken by the student.</span></span> <span data-ttu-id="28f23-110">Isso irá alterar o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="28f23-110">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="28f23-111">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Balde workingResources.</span><span class="sxs-lookup"><span data-stu-id="28f23-111">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="28f23-112">O professor será observando a lista de recursos úteis para a classificação.</span><span class="sxs-lookup"><span data-stu-id="28f23-112">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="28f23-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="28f23-113">Permissions</span></span>
<span data-ttu-id="28f23-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28f23-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28f23-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28f23-116">Permission type</span></span>      | <span data-ttu-id="28f23-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28f23-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28f23-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28f23-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="28f23-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28f23-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="28f23-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28f23-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="28f23-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28f23-121">Not supported.</span></span>  |
|<span data-ttu-id="28f23-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28f23-122">Application</span></span> | <span data-ttu-id="28f23-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28f23-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="28f23-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28f23-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="28f23-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28f23-125">Request headers</span></span>
| <span data-ttu-id="28f23-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28f23-126">Header</span></span>       | <span data-ttu-id="28f23-127">Valor</span><span class="sxs-lookup"><span data-stu-id="28f23-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28f23-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="28f23-128">Authorization</span></span>  | <span data-ttu-id="28f23-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28f23-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28f23-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28f23-131">Request body</span></span>
<span data-ttu-id="28f23-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28f23-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28f23-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f23-133">Response</span></span>
<span data-ttu-id="28f23-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28f23-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28f23-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28f23-136">Example</span></span>
<span data-ttu-id="28f23-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="28f23-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="28f23-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28f23-138">Request</span></span>
<span data-ttu-id="28f23-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28f23-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="28f23-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f23-140">Response</span></span>
<span data-ttu-id="28f23-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28f23-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
