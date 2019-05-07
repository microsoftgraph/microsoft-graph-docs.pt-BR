---
title: Adicionar educationUser a uma educationSchool
description: Adicione um usuário a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3e79796ff7e259fe8ff58f6c9dd908c290e897b5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615825"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="c21c4-103">Adicionar educationUser a uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="c21c4-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="c21c4-104">Adicione um usuário a uma escola.</span><span class="sxs-lookup"><span data-stu-id="c21c4-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c21c4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c21c4-105">Permissions</span></span>
<span data-ttu-id="c21c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c21c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c21c4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c21c4-108">Permission type</span></span>      | <span data-ttu-id="c21c4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c21c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c21c4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c21c4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c21c4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c21c4-111">Not supported.</span></span>  |
|<span data-ttu-id="c21c4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c21c4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c21c4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c21c4-113">Not supported.</span></span>  |
|<span data-ttu-id="c21c4-114">Application</span><span class="sxs-lookup"><span data-stu-id="c21c4-114">Application</span></span> | <span data-ttu-id="c21c4-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c21c4-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c21c4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c21c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c21c4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c21c4-117">Request headers</span></span>
| <span data-ttu-id="c21c4-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c21c4-118">Header</span></span>       | <span data-ttu-id="c21c4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c21c4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c21c4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c21c4-120">Authorization</span></span>  | <span data-ttu-id="c21c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c21c4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c21c4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c21c4-123">Content-Type</span></span>  | <span data-ttu-id="c21c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c21c4-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c21c4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c21c4-125">Request body</span></span>
<span data-ttu-id="c21c4-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="c21c4-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c21c4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c21c4-127">Response</span></span>
<span data-ttu-id="c21c4-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c21c4-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c21c4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c21c4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c21c4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c21c4-130">Request</span></span>
<span data-ttu-id="c21c4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c21c4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="c21c4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c21c4-132">Response</span></span>
<span data-ttu-id="c21c4-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c21c4-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c21c4-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c21c4-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c21c4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c21c4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationschool-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
