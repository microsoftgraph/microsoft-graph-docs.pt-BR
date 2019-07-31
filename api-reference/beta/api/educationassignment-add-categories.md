---
title: Adicionar educationCategories
description: Adicionar um educationCategory existente a este educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b5395ab656d0a5e44b4f3a45f7c136009c5bcc61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955789"
---
# <a name="add-educationcategories"></a><span data-ttu-id="5055a-103">Adicionar educationCategories</span><span class="sxs-lookup"><span data-stu-id="5055a-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5055a-104">Adicione um ou mais objetos [educationCategory](../resources/educationcategory.md) existentes a este [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5055a-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5055a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5055a-105">Permissions</span></span>
<span data-ttu-id="5055a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5055a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5055a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5055a-108">Permission type</span></span>      | <span data-ttu-id="5055a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5055a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5055a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5055a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5055a-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5055a-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5055a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5055a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5055a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5055a-113">Not supported.</span></span>  |
|<span data-ttu-id="5055a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5055a-114">Application</span></span> | <span data-ttu-id="5055a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5055a-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5055a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5055a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5055a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5055a-117">Request headers</span></span>
| <span data-ttu-id="5055a-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5055a-118">Header</span></span>       | <span data-ttu-id="5055a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5055a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5055a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5055a-120">Authorization</span></span>  | <span data-ttu-id="5055a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5055a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5055a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5055a-123">Content-Type</span></span>  | <span data-ttu-id="5055a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5055a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5055a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5055a-125">Request body</span></span>
<span data-ttu-id="5055a-126">No corpo da solicitação, forneça o odata.id dos objetos existentes do [educationCategory](../resources/educationcategory.md) para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="5055a-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="5055a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5055a-127">Response</span></span>
<span data-ttu-id="5055a-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5055a-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5055a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5055a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5055a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5055a-130">Request</span></span>
<span data-ttu-id="5055a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5055a-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="5055a-132">No corpo da solicitação, forneça a odata.id do objeto [educationCategory](../resources/educationcategory.md) existente para adicionar a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="5055a-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="5055a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5055a-133">Response</span></span>
<span data-ttu-id="5055a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5055a-134">The following is an example of the response.</span></span> 

><span data-ttu-id="5055a-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5055a-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5055a-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5055a-136">All of the properties will be returned from an actual call.</span></span>


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
