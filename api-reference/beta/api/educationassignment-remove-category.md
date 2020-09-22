---
title: Remover educationCategory
description: Remover um educationCategory existente deste educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: edcc71fcacf96dacdd9200e48f2ddedbbcda381e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002531"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="07da0-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="07da0-103">Remove educationCategory</span></span>

<span data-ttu-id="07da0-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="07da0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07da0-105">Remover um [educationCategory](../resources/educationcategory.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07da0-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="07da0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07da0-106">Permissions</span></span>
<span data-ttu-id="07da0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07da0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07da0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07da0-109">Permission type</span></span>      | <span data-ttu-id="07da0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07da0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07da0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07da0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="07da0-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07da0-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="07da0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07da0-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="07da0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07da0-114">Not supported.</span></span>  |
|<span data-ttu-id="07da0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07da0-115">Application</span></span> | <span data-ttu-id="07da0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07da0-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="07da0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07da0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="07da0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07da0-118">Request headers</span></span>
| <span data-ttu-id="07da0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07da0-119">Header</span></span>       | <span data-ttu-id="07da0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="07da0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07da0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="07da0-121">Authorization</span></span>  | <span data-ttu-id="07da0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07da0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07da0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07da0-124">Content-Type</span></span>  | <span data-ttu-id="07da0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07da0-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07da0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07da0-126">Request body</span></span>
<span data-ttu-id="07da0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07da0-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="07da0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="07da0-128">Response</span></span>
<span data-ttu-id="07da0-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07da0-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07da0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07da0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07da0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07da0-131">Request</span></span>
<span data-ttu-id="07da0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07da0-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="07da0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="07da0-133">Response</span></span>
<span data-ttu-id="07da0-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07da0-134">The following is an example of the response.</span></span> 

><span data-ttu-id="07da0-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="07da0-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07da0-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07da0-136">All of the properties will be returned from an actual call.</span></span>


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


