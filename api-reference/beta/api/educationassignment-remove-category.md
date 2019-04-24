---
title: Remover educationCategory
description: Remover um educationCategory existente deste educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 9b8d3b2099173911f3ddbadf17a36ba17a4c9027
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464856"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="8f106-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="8f106-103">Remove educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f106-104">Remover um [educationCategory](../resources/educationcategory.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8f106-104">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f106-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f106-105">Permissions</span></span>
<span data-ttu-id="8f106-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f106-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f106-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f106-108">Permission type</span></span>      | <span data-ttu-id="8f106-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f106-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f106-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f106-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8f106-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f106-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8f106-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f106-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8f106-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f106-113">Not supported.</span></span>  |
|<span data-ttu-id="8f106-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f106-114">Application</span></span> | <span data-ttu-id="8f106-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f106-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8f106-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f106-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8f106-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f106-117">Request headers</span></span>
| <span data-ttu-id="8f106-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f106-118">Header</span></span>       | <span data-ttu-id="8f106-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8f106-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f106-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f106-120">Authorization</span></span>  | <span data-ttu-id="8f106-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f106-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8f106-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f106-123">Content-Type</span></span>  | <span data-ttu-id="8f106-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f106-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f106-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f106-125">Request body</span></span>
<span data-ttu-id="8f106-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f106-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8f106-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f106-127">Response</span></span>
<span data-ttu-id="8f106-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f106-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f106-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f106-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f106-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f106-130">Request</span></span>
<span data-ttu-id="8f106-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f106-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="8f106-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f106-132">Response</span></span>
<span data-ttu-id="8f106-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f106-133">The following is an example of the response.</span></span> 

><span data-ttu-id="8f106-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f106-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8f106-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f106-135">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-remove-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
