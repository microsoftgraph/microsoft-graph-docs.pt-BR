---
title: 'educationSubmission: não enviar'
description: 'Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada. Esta ação só pode ser realizada pelo aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 13f21c2442b6ab1715f6c371b32e9d94f99ba125
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322861"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="56a3f-104">educationSubmission: não enviar</span><span class="sxs-lookup"><span data-stu-id="56a3f-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56a3f-105">Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada.</span><span class="sxs-lookup"><span data-stu-id="56a3f-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="56a3f-106">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="56a3f-106">This action can only be taken by the student.</span></span> <span data-ttu-id="56a3f-107">Isso alterará o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="56a3f-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="56a3f-108">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Bucket do workingResources.</span><span class="sxs-lookup"><span data-stu-id="56a3f-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="56a3f-109">O professor examinará a lista de recursos de trabalho para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="56a3f-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="56a3f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="56a3f-110">Permissions</span></span>
<span data-ttu-id="56a3f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56a3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56a3f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56a3f-113">Permission type</span></span>      | <span data-ttu-id="56a3f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56a3f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56a3f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56a3f-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="56a3f-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56a3f-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="56a3f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56a3f-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="56a3f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56a3f-118">Not supported.</span></span>  |
|<span data-ttu-id="56a3f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56a3f-119">Application</span></span> | <span data-ttu-id="56a3f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56a3f-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="56a3f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56a3f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="56a3f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56a3f-122">Request headers</span></span>
| <span data-ttu-id="56a3f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56a3f-123">Header</span></span>       | <span data-ttu-id="56a3f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="56a3f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56a3f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="56a3f-125">Authorization</span></span>  | <span data-ttu-id="56a3f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56a3f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56a3f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56a3f-128">Request body</span></span>
<span data-ttu-id="56a3f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56a3f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56a3f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a3f-130">Response</span></span>
<span data-ttu-id="56a3f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56a3f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56a3f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56a3f-133">Example</span></span>
<span data-ttu-id="56a3f-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="56a3f-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56a3f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56a3f-135">Request</span></span>
<span data-ttu-id="56a3f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56a3f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="56a3f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="56a3f-137">Response</span></span>
<span data-ttu-id="56a3f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56a3f-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
