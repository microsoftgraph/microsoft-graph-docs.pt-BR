---
title: Adicionar educationCategories
description: Adicionar um educationCategory existente a este educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 93dee23d306ccada8d46d5bd91738344f5bd6bf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427841"
---
# <a name="add-educationcategories"></a><span data-ttu-id="dcbff-103">Adicionar educationCategories</span><span class="sxs-lookup"><span data-stu-id="dcbff-103">Add educationCategories</span></span>

<span data-ttu-id="dcbff-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dcbff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcbff-105">Adicione um ou mais objetos [educationCategory](../resources/educationcategory.md) existentes a este [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcbff-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcbff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcbff-106">Permissions</span></span>
<span data-ttu-id="dcbff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcbff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcbff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcbff-109">Permission type</span></span>      | <span data-ttu-id="dcbff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcbff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcbff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcbff-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="dcbff-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcbff-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dcbff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcbff-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dcbff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbff-114">Not supported.</span></span>  |
|<span data-ttu-id="dcbff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcbff-115">Application</span></span> | <span data-ttu-id="dcbff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbff-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="dcbff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dcbff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbff-118">Request headers</span></span>
| <span data-ttu-id="dcbff-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcbff-119">Header</span></span>       | <span data-ttu-id="dcbff-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dcbff-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dcbff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcbff-121">Authorization</span></span>  | <span data-ttu-id="dcbff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcbff-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dcbff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcbff-124">Content-Type</span></span>  | <span data-ttu-id="dcbff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcbff-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dcbff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbff-126">Request body</span></span>
<span data-ttu-id="dcbff-127">No corpo da solicitação, forneça o odata.id dos objetos existentes do [educationCategory](../resources/educationcategory.md) para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="dcbff-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="dcbff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbff-128">Response</span></span>
<span data-ttu-id="dcbff-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dcbff-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dcbff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcbff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcbff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbff-131">Request</span></span>
<span data-ttu-id="dcbff-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbff-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="dcbff-133">No corpo da solicitação, forneça a odata.id do objeto [educationCategory](../resources/educationcategory.md) existente para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="dcbff-133">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="dcbff-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbff-134">Response</span></span>
<span data-ttu-id="dcbff-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbff-135">The following is an example of the response.</span></span> 

><span data-ttu-id="dcbff-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dcbff-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcbff-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcbff-137">All of the properties will be returned from an actual call.</span></span>


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
