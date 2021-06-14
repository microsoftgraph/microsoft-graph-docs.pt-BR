---
title: Excluir educationAssignment
description: Exclua uma atribuição existente. Somente professores em uma classe podem excluir atribuições.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff82696996c9731209b448245515011e2f9baf2a
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911390"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="c2325-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2325-104">Delete educationAssignment</span></span>

<span data-ttu-id="c2325-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2325-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2325-106">Exclua uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="c2325-106">Delete an existing assignment.</span></span> 

<span data-ttu-id="c2325-107">Somente professores em uma classe podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="c2325-107">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2325-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2325-108">Permissions</span></span>

<span data-ttu-id="c2325-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2325-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2325-111">Permission type</span></span>                        | <span data-ttu-id="c2325-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2325-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="c2325-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2325-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2325-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2325-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c2325-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2325-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2325-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2325-116">Not Supported.</span></span>                                          |
| <span data-ttu-id="c2325-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2325-117">Application</span></span>                            | <span data-ttu-id="c2325-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2325-118">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="c2325-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2325-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```

## <a name="request-headers"></a><span data-ttu-id="c2325-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2325-120">Request headers</span></span>

| <span data-ttu-id="c2325-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2325-121">Header</span></span>        | <span data-ttu-id="c2325-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c2325-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c2325-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2325-123">Authorization</span></span> | <span data-ttu-id="c2325-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2325-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2325-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2325-126">Request body</span></span>

<span data-ttu-id="c2325-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="c2325-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2325-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2325-128">Response</span></span>

<span data-ttu-id="c2325-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2325-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2325-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2325-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2325-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2325-132">Request</span></span>

<span data-ttu-id="c2325-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2325-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "delete_educationassignment_1"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
```

### <a name="response"></a><span data-ttu-id="c2325-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2325-134">Response</span></span>
<span data-ttu-id="c2325-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2325-135">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


