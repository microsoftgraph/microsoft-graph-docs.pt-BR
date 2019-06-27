---
title: Adicionar educationClass a educationSchool
description: Adicione uma aula a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 086a8a0393a947c00745208aff46d3d56f016492
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278172"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="29f99-103">Adicionar educationClass a educationSchool</span><span class="sxs-lookup"><span data-stu-id="29f99-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="29f99-104">Adicione uma aula a uma escola.</span><span class="sxs-lookup"><span data-stu-id="29f99-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="29f99-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="29f99-105">Permissions</span></span>
<span data-ttu-id="29f99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29f99-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29f99-108">Permission type</span></span>      | <span data-ttu-id="29f99-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29f99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29f99-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29f99-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="29f99-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29f99-111">Not supported.</span></span>  |
|<span data-ttu-id="29f99-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29f99-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="29f99-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29f99-113">Not supported.</span></span>  |
|<span data-ttu-id="29f99-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29f99-114">Application</span></span> | <span data-ttu-id="29f99-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29f99-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="29f99-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29f99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="29f99-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29f99-117">Request headers</span></span>
| <span data-ttu-id="29f99-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29f99-118">Header</span></span>       | <span data-ttu-id="29f99-119">Valor</span><span class="sxs-lookup"><span data-stu-id="29f99-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29f99-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="29f99-120">Authorization</span></span>  | <span data-ttu-id="29f99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29f99-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29f99-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29f99-123">Content-Type</span></span>  | <span data-ttu-id="29f99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29f99-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29f99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29f99-125">Request body</span></span>
<span data-ttu-id="29f99-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="29f99-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="29f99-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f99-127">Response</span></span>
<span data-ttu-id="29f99-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29f99-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29f99-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29f99-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29f99-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29f99-130">Request</span></span>
<span data-ttu-id="29f99-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29f99-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="29f99-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f99-132">Response</span></span> 
<span data-ttu-id="29f99-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29f99-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="29f99-134">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="29f99-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29f99-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="29f99-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="29f99-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="29f99-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-post-classes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationschool-post-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
