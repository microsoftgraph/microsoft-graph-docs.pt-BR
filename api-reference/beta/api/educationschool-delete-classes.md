---
title: Remover educationClass
description: Exclua uma classe de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 462ba0700a3070c5f01eb8ce9b507a6a3617c177
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529030"
---
# <a name="remove-educationclass"></a><span data-ttu-id="5e098-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="5e098-103">Remove educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e098-104">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="5e098-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e098-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e098-105">Permissions</span></span>
<span data-ttu-id="5e098-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e098-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e098-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e098-108">Permission type</span></span>      | <span data-ttu-id="5e098-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e098-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e098-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e098-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e098-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e098-111">Not supported.</span></span>  |
|<span data-ttu-id="5e098-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e098-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5e098-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e098-113">Not supported.</span></span>  |
|<span data-ttu-id="5e098-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e098-114">Application</span></span> | <span data-ttu-id="5e098-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e098-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5e098-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e098-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5e098-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e098-117">Request headers</span></span>
| <span data-ttu-id="5e098-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e098-118">Header</span></span>       | <span data-ttu-id="5e098-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5e098-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e098-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e098-120">Authorization</span></span>  | <span data-ttu-id="5e098-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e098-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e098-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e098-123">Request body</span></span>
<span data-ttu-id="5e098-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e098-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5e098-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e098-125">Response</span></span>
<span data-ttu-id="5e098-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e098-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e098-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e098-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e098-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e098-128">Request</span></span>
<span data-ttu-id="5e098-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e098-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="5e098-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e098-130">Response</span></span>
<span data-ttu-id="5e098-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e098-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-delete-classes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
