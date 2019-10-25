---
title: 'educationSubmission: versão'
description: " e indica que a gradação foi feita. Esta ação só pode ser feita pelo professor."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ac32d42367d68e405263c66a9bdd980bb652ae5
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726190"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="5ce6e-104">educationSubmission: versão</span><span class="sxs-lookup"><span data-stu-id="5ce6e-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ce6e-105">Esta ação faz com que o [educationOutcome](../resources/educationoutcome.md) inclua notas ou comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-105">This action makes the [educationOutcome](../resources/educationoutcome.md) including any grades or feedback associated with this submission available to the student.</span></span> <span data-ttu-id="5ce6e-106">Isso alterará o status do envio de "enviado" para "lançado" e indicará que a gradação foi feita.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="5ce6e-107">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ce6e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ce6e-108">Permissions</span></span>
<span data-ttu-id="5ce6e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ce6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ce6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ce6e-111">Permission type</span></span>      | <span data-ttu-id="5ce6e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ce6e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ce6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ce6e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ce6e-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ce6e-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="5ce6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ce6e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5ce6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-116">Not supported.</span></span>  |
|<span data-ttu-id="5ce6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ce6e-117">Application</span></span> | <span data-ttu-id="5ce6e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ce6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ce6e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="5ce6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce6e-120">Request headers</span></span>
| <span data-ttu-id="5ce6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ce6e-121">Header</span></span>       | <span data-ttu-id="5ce6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ce6e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ce6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ce6e-123">Authorization</span></span>  | <span data-ttu-id="5ce6e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ce6e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce6e-126">Request body</span></span>
<span data-ttu-id="5ce6e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ce6e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce6e-128">Response</span></span>
<span data-ttu-id="5ce6e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ce6e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ce6e-131">Example</span></span>
<span data-ttu-id="5ce6e-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ce6e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce6e-133">Request</span></span>
<span data-ttu-id="5ce6e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="5ce6e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce6e-135">Response</span></span>
<span data-ttu-id="5ce6e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce6e-136">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
