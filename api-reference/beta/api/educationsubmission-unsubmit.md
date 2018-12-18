---
title: 'educationSubmission: unsubmit'
description: 'Uma ação que indica que um estudante deseja trabalhar no envio da atribuição depois que ele foi ativado. Essa ação só pode ser executada pelo aluno. '
author: dipakboyed
ms.openlocfilehash: a61f2e9c05691266ae9248ca95700f173e0ee0b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304225"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="bd5b7-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="bd5b7-104">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="bd5b7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd5b7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd5b7-107">Uma ação que indica que um estudante deseja trabalhar no envio da atribuição depois que ele foi ativado.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-107">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="bd5b7-108">Essa ação só pode ser executada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-108">This action can only be taken by the student.</span></span> <span data-ttu-id="bd5b7-109">Isso irá alterar o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="bd5b7-109">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="bd5b7-110">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Balde workingResources.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-110">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="bd5b7-111">O professor será observando a lista de recursos úteis para a classificação.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-111">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd5b7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd5b7-112">Permissions</span></span>
<span data-ttu-id="bd5b7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5b7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5b7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd5b7-115">Permission type</span></span>      | <span data-ttu-id="bd5b7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd5b7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd5b7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd5b7-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="bd5b7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd5b7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bd5b7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd5b7-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bd5b7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-120">Not supported.</span></span>  |
|<span data-ttu-id="bd5b7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd5b7-121">Application</span></span> | <span data-ttu-id="bd5b7-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd5b7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd5b7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="bd5b7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd5b7-124">Request headers</span></span>
| <span data-ttu-id="bd5b7-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd5b7-125">Header</span></span>       | <span data-ttu-id="bd5b7-126">Valor</span><span class="sxs-lookup"><span data-stu-id="bd5b7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd5b7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd5b7-127">Authorization</span></span>  | <span data-ttu-id="bd5b7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd5b7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd5b7-130">Request body</span></span>
<span data-ttu-id="bd5b7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd5b7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd5b7-132">Response</span></span>
<span data-ttu-id="bd5b7-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd5b7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd5b7-135">Example</span></span>
<span data-ttu-id="bd5b7-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd5b7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd5b7-137">Request</span></span>
<span data-ttu-id="bd5b7-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="bd5b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd5b7-139">Response</span></span>
<span data-ttu-id="bd5b7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd5b7-140">The following is an example of the response.</span></span>

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
