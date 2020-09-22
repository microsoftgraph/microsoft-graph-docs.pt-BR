---
title: 'educationSubmission: versão'
description: " e indica que a gradação foi feita. Esta ação só pode ser feita pelo professor."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3cb2c5a8388ca10f3c2819d84957cf26eb75f2f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007234"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="4f79a-104">educationSubmission: versão</span><span class="sxs-lookup"><span data-stu-id="4f79a-104">educationSubmission: release</span></span>

<span data-ttu-id="4f79a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f79a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f79a-106">Esta ação faz com que o [educationOutcome](../resources/educationoutcome.md) inclua notas ou comentários associados a esse envio disponível ao aluno.</span><span class="sxs-lookup"><span data-stu-id="4f79a-106">This action makes the [educationOutcome](../resources/educationoutcome.md) including any grades or feedback associated with this submission available to the student.</span></span> <span data-ttu-id="4f79a-107">Isso alterará o status do envio de "enviado" para "lançado" e indicará que a gradação foi feita.</span><span class="sxs-lookup"><span data-stu-id="4f79a-107">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="4f79a-108">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="4f79a-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f79a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f79a-109">Permissions</span></span>
<span data-ttu-id="4f79a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f79a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f79a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f79a-112">Permission type</span></span>      | <span data-ttu-id="4f79a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f79a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f79a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f79a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4f79a-115">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f79a-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="4f79a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f79a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4f79a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f79a-117">Not supported.</span></span>  |
|<span data-ttu-id="4f79a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f79a-118">Application</span></span> | <span data-ttu-id="4f79a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f79a-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4f79a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f79a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="4f79a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f79a-121">Request headers</span></span>
| <span data-ttu-id="4f79a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f79a-122">Header</span></span>       | <span data-ttu-id="4f79a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4f79a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f79a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f79a-124">Authorization</span></span>  | <span data-ttu-id="4f79a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f79a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f79a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f79a-127">Request body</span></span>
<span data-ttu-id="4f79a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f79a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f79a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f79a-129">Response</span></span>
<span data-ttu-id="4f79a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f79a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f79a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f79a-132">Example</span></span>
<span data-ttu-id="4f79a-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4f79a-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f79a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f79a-134">Request</span></span>
<span data-ttu-id="4f79a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f79a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="4f79a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f79a-136">Response</span></span>
<span data-ttu-id="4f79a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f79a-137">The following is an example of the response.</span></span>

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


