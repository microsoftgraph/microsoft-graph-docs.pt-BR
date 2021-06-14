---
title: Excluir educationCategory
description: Exclua uma categoria existente.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eed94985bfa1de66215f7afd1ca64d236846a118
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911383"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="ac85e-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="ac85e-103">Delete educationCategory</span></span>

<span data-ttu-id="ac85e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac85e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac85e-105">Excluir uma categoria [existente](../resources/educationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ac85e-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac85e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac85e-106">Permissions</span></span>

<span data-ttu-id="ac85e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac85e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac85e-109">Permission type</span></span>                        | <span data-ttu-id="ac85e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac85e-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="ac85e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac85e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac85e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac85e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="ac85e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac85e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac85e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac85e-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="ac85e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac85e-115">Application</span></span>                            | <span data-ttu-id="ac85e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac85e-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="ac85e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac85e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac85e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac85e-118">Request headers</span></span>

| <span data-ttu-id="ac85e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac85e-119">Header</span></span>        | <span data-ttu-id="ac85e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ac85e-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ac85e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac85e-121">Authorization</span></span> | <span data-ttu-id="ac85e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac85e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac85e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac85e-124">Request body</span></span>

<span data-ttu-id="ac85e-125">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="ac85e-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac85e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac85e-126">Response</span></span>

<span data-ttu-id="ac85e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac85e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac85e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac85e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac85e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac85e-130">Request</span></span>

<span data-ttu-id="ac85e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac85e-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```

### <a name="response"></a><span data-ttu-id="ac85e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac85e-132">Response</span></span>

<span data-ttu-id="ac85e-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac85e-133">The following is an example of the response.</span></span> 

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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


