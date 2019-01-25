---
title: 'educationSubmission: retornar'
description: Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b1772788230b5220b3bdc6813b122d1158e26ab2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511237"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="8327f-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="8327f-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8327f-104">Esta ação faz com que o nível e os comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="8327f-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="8327f-105">Isso irá alterar o status do envio de "enviado" a "retornado" e indica que o comentário for fornecido ou classificação é feito.</span><span class="sxs-lookup"><span data-stu-id="8327f-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="8327f-106">Essa ação só pode ser feita com o professor.</span><span class="sxs-lookup"><span data-stu-id="8327f-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="8327f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8327f-107">Permissions</span></span>
<span data-ttu-id="8327f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8327f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8327f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8327f-110">Permission type</span></span>      | <span data-ttu-id="8327f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8327f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8327f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8327f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8327f-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8327f-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8327f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8327f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8327f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8327f-115">Not supported.</span></span>  |
|<span data-ttu-id="8327f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8327f-116">Application</span></span> | <span data-ttu-id="8327f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8327f-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8327f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8327f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="8327f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8327f-119">Request headers</span></span>
| <span data-ttu-id="8327f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8327f-120">Header</span></span>       | <span data-ttu-id="8327f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8327f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8327f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8327f-122">Authorization</span></span>  | <span data-ttu-id="8327f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8327f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8327f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8327f-125">Request body</span></span>
<span data-ttu-id="8327f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8327f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8327f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327f-127">Response</span></span>
<span data-ttu-id="8327f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8327f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8327f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8327f-130">Example</span></span>
<span data-ttu-id="8327f-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8327f-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8327f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8327f-132">Request</span></span>
<span data-ttu-id="8327f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8327f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="8327f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327f-134">Response</span></span>
<span data-ttu-id="8327f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8327f-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
