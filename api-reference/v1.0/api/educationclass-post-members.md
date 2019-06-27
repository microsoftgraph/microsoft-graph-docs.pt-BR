---
title: Adicionar um aluno
description: Adicione um membro a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac2cca18a733ac99bc8aadb9d0bbaae9a6e69455
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275149"
---
# <a name="add-a-student"></a><span data-ttu-id="ebc84-103">Adicionar um aluno</span><span class="sxs-lookup"><span data-stu-id="ebc84-103">Add a student</span></span>

<span data-ttu-id="ebc84-104">Adicione um membro a uma aula.</span><span class="sxs-lookup"><span data-stu-id="ebc84-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebc84-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebc84-105">Permissions</span></span>
<span data-ttu-id="ebc84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebc84-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebc84-108">Permission type</span></span>      | <span data-ttu-id="ebc84-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebc84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebc84-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebc84-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebc84-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc84-111">Not supported.</span></span>  |
|<span data-ttu-id="ebc84-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebc84-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ebc84-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc84-113">Not supported.</span></span>  |
|<span data-ttu-id="ebc84-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc84-114">Application</span></span> | <span data-ttu-id="ebc84-115">EduRoster. ReadWrite. All mais member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="ebc84-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ebc84-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ebc84-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc84-117">Request headers</span></span>
| <span data-ttu-id="ebc84-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebc84-118">Header</span></span>       | <span data-ttu-id="ebc84-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ebc84-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebc84-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc84-120">Authorization</span></span>  | <span data-ttu-id="ebc84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebc84-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ebc84-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebc84-123">Content-Type</span></span>  | <span data-ttu-id="ebc84-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ebc84-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebc84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc84-125">Request body</span></span>
<span data-ttu-id="ebc84-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="ebc84-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ebc84-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc84-127">Response</span></span>
<span data-ttu-id="ebc84-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc84-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebc84-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebc84-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebc84-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc84-130">Request</span></span>
<span data-ttu-id="ebc84-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebc84-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="ebc84-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc84-132">Response</span></span>
<span data-ttu-id="ebc84-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc84-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ebc84-134">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="ebc84-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebc84-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc84-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ebc84-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ebc84-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
