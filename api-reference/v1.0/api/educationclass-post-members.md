---
title: Adicionar um aluno
description: Adicione um membro a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4c859c6fa47b9f53eeced4b944822ba8a089417c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517562"
---
# <a name="add-a-student"></a><span data-ttu-id="85813-103">Adicionar um aluno</span><span class="sxs-lookup"><span data-stu-id="85813-103">Add a student</span></span>

<span data-ttu-id="85813-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85813-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85813-105">Adicione um membro a uma aula.</span><span class="sxs-lookup"><span data-stu-id="85813-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="85813-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85813-106">Permissions</span></span>
<span data-ttu-id="85813-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85813-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85813-109">Permission type</span></span>      | <span data-ttu-id="85813-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85813-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85813-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85813-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="85813-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85813-112">Not supported.</span></span>  |
|<span data-ttu-id="85813-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85813-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="85813-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85813-114">Not supported.</span></span>  |
|<span data-ttu-id="85813-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85813-115">Application</span></span> | <span data-ttu-id="85813-116">EduRoster. ReadWrite. All mais member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="85813-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="85813-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85813-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="85813-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85813-118">Request headers</span></span>
| <span data-ttu-id="85813-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85813-119">Header</span></span>       | <span data-ttu-id="85813-120">Valor</span><span class="sxs-lookup"><span data-stu-id="85813-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85813-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85813-121">Authorization</span></span>  | <span data-ttu-id="85813-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85813-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85813-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85813-124">Content-Type</span></span>  | <span data-ttu-id="85813-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85813-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85813-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85813-126">Request body</span></span>
<span data-ttu-id="85813-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="85813-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="85813-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85813-128">Response</span></span>
<span data-ttu-id="85813-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85813-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85813-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85813-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85813-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85813-131">Request</span></span>
<span data-ttu-id="85813-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85813-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85813-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85813-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="85813-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85813-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85813-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85813-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="85813-136">C#</span><span class="sxs-lookup"><span data-stu-id="85813-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85813-137">Java</span><span class="sxs-lookup"><span data-stu-id="85813-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85813-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="85813-138">Response</span></span>
<span data-ttu-id="85813-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85813-139">The following is an example of the response.</span></span> 


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
