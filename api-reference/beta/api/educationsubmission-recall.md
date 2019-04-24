---
title: 'educationSubmission: rechamar'
description: 'Indica que um aluno deseja fazer um envio. Esta ação só pode ser feita por um aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0be94d2888223ca31e37b71e490c4a9fdc28b7d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457625"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="38029-104">educationSubmission: rechamar</span><span class="sxs-lookup"><span data-stu-id="38029-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38029-105">Indica que um aluno deseja fazer um envio.</span><span class="sxs-lookup"><span data-stu-id="38029-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="38029-106">Esta ação só pode ser feita por um aluno.</span><span class="sxs-lookup"><span data-stu-id="38029-106">This action can only be done by a student.</span></span> <span data-ttu-id="38029-107">Ele alterará o status do envio de "enviado" de volta para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="38029-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="38029-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="38029-108">Permissions</span></span>
<span data-ttu-id="38029-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38029-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38029-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38029-111">Permission type</span></span>      | <span data-ttu-id="38029-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38029-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38029-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38029-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="38029-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38029-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="38029-115">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38029-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38029-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="38029-116">Not supported</span></span>  |
|<span data-ttu-id="38029-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38029-117">Application</span></span> |<span data-ttu-id="38029-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38029-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="38029-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38029-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="38029-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38029-120">Request headers</span></span>
| <span data-ttu-id="38029-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38029-121">Header</span></span>       | <span data-ttu-id="38029-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38029-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38029-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38029-123">Authorization</span></span>  | <span data-ttu-id="38029-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38029-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38029-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38029-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="38029-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="38029-127">Response</span></span>
<span data-ttu-id="38029-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38029-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38029-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38029-130">Example</span></span>
<span data-ttu-id="38029-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="38029-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38029-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38029-132">Request</span></span>
<span data-ttu-id="38029-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38029-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="38029-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="38029-134">Response</span></span>
<span data-ttu-id="38029-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38029-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-recall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
