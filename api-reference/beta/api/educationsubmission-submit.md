---
title: 'educationSubmission: enviar'
description: Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição. Esta ação só pode ser realizada pelo aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f67e5b07ed1093ee63e9b6fdf7647fa6891dacc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464723"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="f1084-104">educationSubmission: enviar</span><span class="sxs-lookup"><span data-stu-id="f1084-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1084-105">Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição.</span><span class="sxs-lookup"><span data-stu-id="f1084-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="f1084-106">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="f1084-106">This action can only be taken by the student.</span></span> <span data-ttu-id="f1084-107">Isso alterará o status do envio de "trabalho" para "enviado".</span><span class="sxs-lookup"><span data-stu-id="f1084-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="f1084-108">Durante o processo de envio, todos os recursos serão copiados para o Bucket submittedResources.</span><span class="sxs-lookup"><span data-stu-id="f1084-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="f1084-109">O professor examinará a lista de recursos enviados para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="f1084-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1084-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1084-110">Permissions</span></span>
<span data-ttu-id="f1084-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1084-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1084-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1084-113">Permission type</span></span>      | <span data-ttu-id="f1084-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1084-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1084-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1084-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1084-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1084-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f1084-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1084-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1084-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1084-118">Not supported.</span></span>  |
|<span data-ttu-id="f1084-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1084-119">Application</span></span> | <span data-ttu-id="f1084-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1084-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f1084-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1084-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="f1084-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1084-122">Request headers</span></span>
| <span data-ttu-id="f1084-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1084-123">Header</span></span>       | <span data-ttu-id="f1084-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f1084-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1084-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1084-125">Authorization</span></span>  | <span data-ttu-id="f1084-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1084-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1084-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1084-128">Request body</span></span>
<span data-ttu-id="f1084-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1084-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1084-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1084-130">Response</span></span>
<span data-ttu-id="f1084-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1084-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1084-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1084-133">Example</span></span>
<span data-ttu-id="f1084-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f1084-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1084-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1084-135">Request</span></span>
<span data-ttu-id="f1084-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1084-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="f1084-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1084-137">Response</span></span>
<span data-ttu-id="f1084-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1084-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
