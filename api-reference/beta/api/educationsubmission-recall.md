---
title: 'educationSubmission: rechamar'
description: 'Indica que um aluno deseja fazer um envio. Esta ação só pode ser feita por um aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 606a2a5325da9aed6203303e40ad5b3b95f0d7d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007228"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="c5471-104">educationSubmission: rechamar</span><span class="sxs-lookup"><span data-stu-id="c5471-104">educationSubmission: recall</span></span>

<span data-ttu-id="c5471-105">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c5471-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5471-106">Indica que um aluno deseja fazer um envio.</span><span class="sxs-lookup"><span data-stu-id="c5471-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="c5471-107">Esta ação só pode ser feita por um aluno.</span><span class="sxs-lookup"><span data-stu-id="c5471-107">This action can only be done by a student.</span></span> <span data-ttu-id="c5471-108">Ele alterará o status do envio de "enviado" de volta para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="c5471-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="c5471-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5471-109">Permissions</span></span>

<span data-ttu-id="c5471-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5471-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5471-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5471-112">Permission type</span></span>                        | <span data-ttu-id="c5471-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5471-113">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="c5471-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5471-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5471-115">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5471-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c5471-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5471-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5471-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c5471-117">Not supported</span></span>                                           |
| <span data-ttu-id="c5471-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5471-118">Application</span></span>                            | <span data-ttu-id="c5471-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5471-119">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="c5471-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5471-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a><span data-ttu-id="c5471-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5471-121">Request headers</span></span>

| <span data-ttu-id="c5471-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5471-122">Header</span></span>        | <span data-ttu-id="c5471-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c5471-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c5471-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5471-124">Authorization</span></span> | <span data-ttu-id="c5471-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5471-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5471-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5471-127">Response</span></span>

<span data-ttu-id="c5471-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5471-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5471-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5471-130">Example</span></span>

<span data-ttu-id="c5471-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c5471-131">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c5471-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5471-132">Request</span></span>

<span data-ttu-id="c5471-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5471-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="c5471-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5471-134">Response</span></span>

<span data-ttu-id="c5471-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5471-135">The following is an example of the response.</span></span>

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


