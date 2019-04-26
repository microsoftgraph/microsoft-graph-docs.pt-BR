---
title: 'educationSubmission: versão'
description: " e indica que a gradação foi feita. Esta ação só pode ser feita pelo professor."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d2fe5403534fc6e7140c7e0b8e8731707feac5b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322844"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="8a44a-104">educationSubmission: versão</span><span class="sxs-lookup"><span data-stu-id="8a44a-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a44a-105">Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.</span><span class="sxs-lookup"><span data-stu-id="8a44a-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="8a44a-106">Isso alterará o status do envio de "enviado" para "lançado" e indicará que a gradação foi feita.</span><span class="sxs-lookup"><span data-stu-id="8a44a-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="8a44a-107">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="8a44a-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a44a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a44a-108">Permissions</span></span>
<span data-ttu-id="8a44a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a44a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a44a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a44a-111">Permission type</span></span>      | <span data-ttu-id="8a44a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a44a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a44a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a44a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a44a-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a44a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8a44a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a44a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a44a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a44a-116">Not supported.</span></span>  |
|<span data-ttu-id="8a44a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a44a-117">Application</span></span> | <span data-ttu-id="8a44a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a44a-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a44a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a44a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="8a44a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a44a-120">Request headers</span></span>
| <span data-ttu-id="8a44a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a44a-121">Header</span></span>       | <span data-ttu-id="8a44a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a44a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a44a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a44a-123">Authorization</span></span>  | <span data-ttu-id="8a44a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a44a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a44a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a44a-126">Request body</span></span>
<span data-ttu-id="8a44a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a44a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a44a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a44a-128">Response</span></span>
<span data-ttu-id="8a44a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a44a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a44a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a44a-131">Example</span></span>
<span data-ttu-id="8a44a-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8a44a-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a44a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a44a-133">Request</span></span>
<span data-ttu-id="8a44a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a44a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="8a44a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a44a-135">Response</span></span>
<span data-ttu-id="8a44a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a44a-136">The following is an example of the response.</span></span>

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
