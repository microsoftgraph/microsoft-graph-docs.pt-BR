---
title: Remover educationCategory
description: Remover uma educationCategory existente deste educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c60fd9a3de1d6c66d326ecb0d87416556839c72e
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911385"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="f02df-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="f02df-103">Remove educationCategory</span></span>

<span data-ttu-id="f02df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f02df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f02df-105">Remover uma [educationCategory](../resources/educationcategory.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f02df-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f02df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f02df-106">Permissions</span></span>
<span data-ttu-id="f02df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f02df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f02df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f02df-109">Permission type</span></span>      | <span data-ttu-id="f02df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f02df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f02df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f02df-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f02df-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f02df-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f02df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f02df-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f02df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f02df-114">Not supported.</span></span>  |
|<span data-ttu-id="f02df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f02df-115">Application</span></span> | <span data-ttu-id="f02df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f02df-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f02df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f02df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f02df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f02df-118">Request headers</span></span>
| <span data-ttu-id="f02df-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f02df-119">Header</span></span>       | <span data-ttu-id="f02df-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f02df-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f02df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f02df-121">Authorization</span></span>  | <span data-ttu-id="f02df-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f02df-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f02df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f02df-124">Content-Type</span></span>  | <span data-ttu-id="f02df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f02df-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f02df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f02df-126">Request body</span></span>
<span data-ttu-id="f02df-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="f02df-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f02df-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f02df-128">Response</span></span>
<span data-ttu-id="f02df-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f02df-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f02df-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f02df-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f02df-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f02df-131">Request</span></span>
<span data-ttu-id="f02df-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f02df-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["ec98f158-341d-4fea-9f8c-14a250d489ac"],
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

### <a name="response"></a><span data-ttu-id="f02df-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f02df-133">Response</span></span>
<span data-ttu-id="f02df-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f02df-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content

{
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


