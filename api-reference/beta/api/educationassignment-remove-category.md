---
title: Remover educationCategory
description: Remover uma educationCategory existente deste educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: edf054ba1d7b81800a75e260c5a2357ae2d9bcba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044183"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="25e7a-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="25e7a-103">Remove educationCategory</span></span>

<span data-ttu-id="25e7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e7a-105">Remover uma [educationCategory](../resources/educationcategory.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="25e7a-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25e7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25e7a-106">Permissions</span></span>
<span data-ttu-id="25e7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25e7a-109">Permission type</span></span>      | <span data-ttu-id="25e7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25e7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25e7a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="25e7a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25e7a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="25e7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25e7a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="25e7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25e7a-114">Not supported.</span></span>  |
|<span data-ttu-id="25e7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25e7a-115">Application</span></span> | <span data-ttu-id="25e7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25e7a-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="25e7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25e7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="25e7a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25e7a-118">Request headers</span></span>
| <span data-ttu-id="25e7a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25e7a-119">Header</span></span>       | <span data-ttu-id="25e7a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="25e7a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25e7a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25e7a-121">Authorization</span></span>  | <span data-ttu-id="25e7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25e7a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="25e7a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25e7a-124">Content-Type</span></span>  | <span data-ttu-id="25e7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25e7a-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25e7a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25e7a-126">Request body</span></span>
<span data-ttu-id="25e7a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25e7a-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="25e7a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="25e7a-128">Response</span></span>
<span data-ttu-id="25e7a-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25e7a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25e7a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25e7a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25e7a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25e7a-131">Request</span></span>
<span data-ttu-id="25e7a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25e7a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="25e7a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="25e7a-133">Response</span></span>
<span data-ttu-id="25e7a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25e7a-134">The following is an example of the response.</span></span> 

><span data-ttu-id="25e7a-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="25e7a-135">**Note:** The response object shown here might be shortened for readability.</span></span>


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
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


