---
title: Adicionar um aluno
description: Adicione um membro a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ff099a826e5b361bd86d5e090e8f8ea65fb644f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370414"
---
# <a name="add-a-student"></a><span data-ttu-id="5e531-103">Adicionar um aluno</span><span class="sxs-lookup"><span data-stu-id="5e531-103">Add a student</span></span>

<span data-ttu-id="5e531-104">Adicione um membro a uma aula.</span><span class="sxs-lookup"><span data-stu-id="5e531-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e531-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e531-105">Permissions</span></span>
<span data-ttu-id="5e531-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e531-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e531-108">Permission type</span></span>      | <span data-ttu-id="5e531-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e531-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e531-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e531-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e531-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e531-111">Not supported.</span></span>  |
|<span data-ttu-id="5e531-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e531-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5e531-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e531-113">Not supported.</span></span>  |
|<span data-ttu-id="5e531-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e531-114">Application</span></span> | <span data-ttu-id="5e531-115">EduRoster. ReadWrite. All mais member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="5e531-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5e531-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e531-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5e531-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e531-117">Request headers</span></span>
| <span data-ttu-id="5e531-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e531-118">Header</span></span>       | <span data-ttu-id="5e531-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5e531-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e531-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e531-120">Authorization</span></span>  | <span data-ttu-id="5e531-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e531-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e531-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e531-123">Content-Type</span></span>  | <span data-ttu-id="5e531-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5e531-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e531-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e531-125">Request body</span></span>
<span data-ttu-id="5e531-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="5e531-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5e531-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e531-127">Response</span></span>
<span data-ttu-id="5e531-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e531-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e531-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e531-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e531-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e531-130">Request</span></span>
<span data-ttu-id="5e531-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e531-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e531-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e531-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e531-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e531-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e531-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5e531-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="5e531-135">C#</span><span class="sxs-lookup"><span data-stu-id="5e531-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5e531-136">Java</span><span class="sxs-lookup"><span data-stu-id="5e531-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e531-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e531-137">Response</span></span>
<span data-ttu-id="5e531-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e531-138">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
