---
title: 'educationSubmission: enviar'
description: . Durante o processo de envio, todos os recursos serão copiados para o Balde submittedResources. O professor será observando a lista de recursos enviados para a classificação.
ms.openlocfilehash: 566948278ffacb1169842c49aa11c78cba0a5f3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034898"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="db815-105">educationSubmission: enviar</span><span class="sxs-lookup"><span data-stu-id="db815-105">educationSubmission: submit</span></span>

> <span data-ttu-id="db815-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db815-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db815-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db815-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db815-108">Uma ação que indica que um estudante é feito com o trabalho e está pronto para informar na atribuição.</span><span class="sxs-lookup"><span data-stu-id="db815-108">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="db815-109">Essa ação só pode ser executada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="db815-109">This action can only be taken by the student.</span></span> <span data-ttu-id="db815-110">Isso alterará o status do envio de "trabalho" para "enviado".</span><span class="sxs-lookup"><span data-stu-id="db815-110">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="db815-111">Durante o processo de envio, todos os recursos serão copiados para o Balde submittedResources.</span><span class="sxs-lookup"><span data-stu-id="db815-111">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="db815-112">O professor será observando a lista de recursos enviados para a classificação.</span><span class="sxs-lookup"><span data-stu-id="db815-112">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="db815-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="db815-113">Permissions</span></span>
<span data-ttu-id="db815-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db815-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db815-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db815-116">Permission type</span></span>      | <span data-ttu-id="db815-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db815-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db815-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db815-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="db815-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db815-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="db815-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db815-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="db815-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db815-121">Not supported.</span></span>  |
|<span data-ttu-id="db815-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db815-122">Application</span></span> | <span data-ttu-id="db815-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db815-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="db815-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db815-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="db815-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db815-125">Request headers</span></span>
| <span data-ttu-id="db815-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db815-126">Header</span></span>       | <span data-ttu-id="db815-127">Valor</span><span class="sxs-lookup"><span data-stu-id="db815-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db815-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="db815-128">Authorization</span></span>  | <span data-ttu-id="db815-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db815-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db815-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db815-131">Request body</span></span>
<span data-ttu-id="db815-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db815-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db815-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="db815-133">Response</span></span>
<span data-ttu-id="db815-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db815-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db815-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db815-136">Example</span></span>
<span data-ttu-id="db815-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="db815-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db815-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db815-138">Request</span></span>
<span data-ttu-id="db815-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db815-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="db815-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="db815-140">Response</span></span>
<span data-ttu-id="db815-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db815-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->