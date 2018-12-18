---
title: 'educationSubmission: enviar'
description: Uma ação que indica que um estudante é feito com o trabalho e está pronto para informar na atribuição. Essa ação só pode ser executada pelo aluno.
author: dipakboyed
ms.openlocfilehash: 25fc24823081c6f148617ad31d0f7b797b0e2a80
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343327"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="93d80-104">educationSubmission: enviar</span><span class="sxs-lookup"><span data-stu-id="93d80-104">educationSubmission: submit</span></span>

> <span data-ttu-id="93d80-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93d80-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93d80-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93d80-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93d80-107">Uma ação que indica que um estudante é feito com o trabalho e está pronto para informar na atribuição.</span><span class="sxs-lookup"><span data-stu-id="93d80-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="93d80-108">Essa ação só pode ser executada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="93d80-108">This action can only be taken by the student.</span></span> <span data-ttu-id="93d80-109">Isso alterará o status do envio de "trabalho" para "enviado".</span><span class="sxs-lookup"><span data-stu-id="93d80-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="93d80-110">Durante o processo de envio, todos os recursos serão copiados para o Balde submittedResources.</span><span class="sxs-lookup"><span data-stu-id="93d80-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="93d80-111">O professor será observando a lista de recursos enviados para a classificação.</span><span class="sxs-lookup"><span data-stu-id="93d80-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d80-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="93d80-112">Permissions</span></span>
<span data-ttu-id="93d80-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d80-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d80-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93d80-115">Permission type</span></span>      | <span data-ttu-id="93d80-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93d80-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d80-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93d80-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="93d80-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93d80-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="93d80-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93d80-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93d80-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93d80-120">Not supported.</span></span>  |
|<span data-ttu-id="93d80-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93d80-121">Application</span></span> | <span data-ttu-id="93d80-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93d80-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="93d80-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93d80-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="93d80-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93d80-124">Request headers</span></span>
| <span data-ttu-id="93d80-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93d80-125">Header</span></span>       | <span data-ttu-id="93d80-126">Valor</span><span class="sxs-lookup"><span data-stu-id="93d80-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93d80-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="93d80-127">Authorization</span></span>  | <span data-ttu-id="93d80-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93d80-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93d80-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93d80-130">Request body</span></span>
<span data-ttu-id="93d80-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93d80-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d80-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d80-132">Response</span></span>
<span data-ttu-id="93d80-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93d80-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93d80-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93d80-135">Example</span></span>
<span data-ttu-id="93d80-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="93d80-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="93d80-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93d80-137">Request</span></span>
<span data-ttu-id="93d80-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93d80-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="93d80-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d80-139">Response</span></span>
<span data-ttu-id="93d80-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93d80-140">The following is an example of the response.</span></span>

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