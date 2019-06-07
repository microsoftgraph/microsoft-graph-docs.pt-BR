---
title: 'educationSubmission: rechamar'
description: 'Indica que um aluno deseja fazer um envio. Esta ação só pode ser feita por um aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fc365e61def62dbbf65c47d9bc0163f15be9475d
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34749958"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="79505-104">educationSubmission: rechamar</span><span class="sxs-lookup"><span data-stu-id="79505-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79505-105">Indica que um aluno deseja fazer um envio.</span><span class="sxs-lookup"><span data-stu-id="79505-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="79505-106">Esta ação só pode ser feita por um aluno.</span><span class="sxs-lookup"><span data-stu-id="79505-106">This action can only be done by a student.</span></span> <span data-ttu-id="79505-107">Ele alterará o status do envio de "enviado" de volta para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="79505-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="79505-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="79505-108">Permissions</span></span>

<span data-ttu-id="79505-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79505-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79505-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79505-111">Permission type</span></span>                        | <span data-ttu-id="79505-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79505-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="79505-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79505-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="79505-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79505-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="79505-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79505-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79505-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="79505-116">Not supported</span></span>                                           |
| <span data-ttu-id="79505-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79505-117">Application</span></span>                            | <span data-ttu-id="79505-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79505-118">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="79505-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79505-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a><span data-ttu-id="79505-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79505-120">Request headers</span></span>

| <span data-ttu-id="79505-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79505-121">Header</span></span>        | <span data-ttu-id="79505-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79505-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="79505-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79505-123">Authorization</span></span> | <span data-ttu-id="79505-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79505-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="79505-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="79505-126">Response</span></span>

<span data-ttu-id="79505-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79505-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79505-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79505-129">Example</span></span>

<span data-ttu-id="79505-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="79505-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="79505-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79505-131">Request</span></span>

<span data-ttu-id="79505-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79505-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="79505-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="79505-133">Response</span></span>

<span data-ttu-id="79505-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79505-134">The following is an example of the response.</span></span>

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
  "suppressions": []
}
-->
