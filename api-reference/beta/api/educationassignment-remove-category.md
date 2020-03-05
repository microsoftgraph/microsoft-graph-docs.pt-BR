---
title: Remover educationCategory
description: Remover um educationCategory existente deste educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d154f4c46eaeaa84807966b3f78947e09ba01be0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427337"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="972d7-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="972d7-103">Remove educationCategory</span></span>

<span data-ttu-id="972d7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="972d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="972d7-105">Remover um [educationCategory](../resources/educationcategory.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="972d7-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="972d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="972d7-106">Permissions</span></span>
<span data-ttu-id="972d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="972d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="972d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="972d7-109">Permission type</span></span>      | <span data-ttu-id="972d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="972d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="972d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="972d7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="972d7-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="972d7-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="972d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="972d7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="972d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="972d7-114">Not supported.</span></span>  |
|<span data-ttu-id="972d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="972d7-115">Application</span></span> | <span data-ttu-id="972d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="972d7-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="972d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="972d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="972d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="972d7-118">Request headers</span></span>
| <span data-ttu-id="972d7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="972d7-119">Header</span></span>       | <span data-ttu-id="972d7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="972d7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="972d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="972d7-121">Authorization</span></span>  | <span data-ttu-id="972d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="972d7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="972d7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="972d7-124">Content-Type</span></span>  | <span data-ttu-id="972d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="972d7-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="972d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="972d7-126">Request body</span></span>
<span data-ttu-id="972d7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="972d7-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="972d7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="972d7-128">Response</span></span>
<span data-ttu-id="972d7-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="972d7-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="972d7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="972d7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="972d7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="972d7-131">Request</span></span>
<span data-ttu-id="972d7-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="972d7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="972d7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="972d7-133">Response</span></span>
<span data-ttu-id="972d7-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="972d7-134">The following is an example of the response.</span></span> 

><span data-ttu-id="972d7-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="972d7-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="972d7-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="972d7-136">All of the properties will be returned from an actual call.</span></span>


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
