---
title: Criar educationCategories
description: Adicionar uma educationCategory existente a um educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 600c73d8fdae1bc9946f31cf472618591d79de6d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912157"
---
# <a name="create-educationcategories"></a><span data-ttu-id="ff074-103">Criar educationCategories</span><span class="sxs-lookup"><span data-stu-id="ff074-103">Create educationCategories</span></span>

<span data-ttu-id="ff074-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff074-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff074-105">Adicionar um ou mais objetos [educationCategory](../resources/educationcategory.md) existentes ao [educationAssignment especificado.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ff074-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to the specified  [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff074-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff074-106">Permissions</span></span>
<span data-ttu-id="ff074-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff074-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff074-109">Permission type</span></span>      | <span data-ttu-id="ff074-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff074-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff074-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff074-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff074-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff074-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ff074-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff074-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ff074-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff074-114">Not supported.</span></span>  |
|<span data-ttu-id="ff074-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff074-115">Application</span></span> | <span data-ttu-id="ff074-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff074-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ff074-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff074-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ff074-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff074-118">Request headers</span></span>
| <span data-ttu-id="ff074-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff074-119">Header</span></span>       | <span data-ttu-id="ff074-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ff074-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff074-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff074-121">Authorization</span></span>  | <span data-ttu-id="ff074-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff074-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff074-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff074-124">Content-Type</span></span>  | <span data-ttu-id="ff074-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff074-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff074-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff074-126">Request body</span></span>
<span data-ttu-id="ff074-127">No corpo da solicitação, odata.id os objetos [educationCategory](../resources/educationcategory.md) existentes para adicionar a esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="ff074-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="ff074-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff074-128">Response</span></span>
<span data-ttu-id="ff074-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff074-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff074-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff074-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff074-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff074-131">Request</span></span>
<span data-ttu-id="ff074-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff074-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_educationcategory_to_educationassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="ff074-133">No corpo da solicitação, fornece o odata.id do objeto [educationCategory](../resources/educationcategory.md) existente para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="ff074-133">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>

### <a name="response"></a><span data-ttu-id="ff074-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff074-134">Response</span></span>
<span data-ttu-id="ff074-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff074-135">The following is an example of the response.</span></span> 

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
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


