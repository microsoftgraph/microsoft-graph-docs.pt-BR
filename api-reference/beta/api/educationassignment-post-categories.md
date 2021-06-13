---
title: Criar educationCategories
description: Adicionar uma educationCategory existente a um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 847e720e65da2604a1188d9854e4e10320d0d181
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912961"
---
# <a name="create-educationcategories"></a><span data-ttu-id="f9f66-103">Criar educationCategories</span><span class="sxs-lookup"><span data-stu-id="f9f66-103">Create educationCategories</span></span>

<span data-ttu-id="f9f66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9f66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f66-105">Adicione um ou mais objetos [educationCategory](../resources/educationcategory.md) existentes a [este educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9f66-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f66-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9f66-106">Permissions</span></span>
<span data-ttu-id="f9f66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f66-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f66-109">Permission type</span></span>      | <span data-ttu-id="f9f66-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9f66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9f66-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f66-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f9f66-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f66-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f9f66-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f66-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f9f66-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f66-114">Not supported.</span></span>  |
|<span data-ttu-id="f9f66-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f66-115">Application</span></span> | <span data-ttu-id="f9f66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f66-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f9f66-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f9f66-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f66-118">Request headers</span></span>
| <span data-ttu-id="f9f66-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9f66-119">Header</span></span>       | <span data-ttu-id="f9f66-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f9f66-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9f66-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f66-121">Authorization</span></span>  | <span data-ttu-id="f9f66-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f66-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9f66-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9f66-124">Content-Type</span></span>  | <span data-ttu-id="f9f66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f66-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9f66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f66-126">Request body</span></span>
<span data-ttu-id="f9f66-127">No corpo da solicitação, odata.id os objetos [educationCategory](../resources/educationcategory.md) existentes para adicionar a esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="f9f66-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="f9f66-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f66-128">Response</span></span>
<span data-ttu-id="f9f66-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9f66-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9f66-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9f66-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9f66-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f66-131">Request</span></span>
<span data-ttu-id="f9f66-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f66-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="f9f66-133">No corpo da solicitação, fornece o odata.id do objeto [educationCategory](../resources/educationcategory.md) existente para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="f9f66-133">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="f9f66-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f66-134">Response</span></span>
<span data-ttu-id="f9f66-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f66-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f9f66-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9f66-136">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
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


