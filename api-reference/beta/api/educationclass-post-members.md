---
title: Adicionar um aluno
description: Adicione um membro a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e5958a9b737ee228755ca7bd6153dff108b49245
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785981"
---
# <a name="add-a-student"></a><span data-ttu-id="74195-103">Adicionar um aluno</span><span class="sxs-lookup"><span data-stu-id="74195-103">Add a student</span></span>

<span data-ttu-id="74195-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74195-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74195-105">Adicione um membro a uma aula.</span><span class="sxs-lookup"><span data-stu-id="74195-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="74195-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="74195-106">Permissions</span></span>
<span data-ttu-id="74195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74195-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74195-109">Permission type</span></span>      | <span data-ttu-id="74195-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74195-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74195-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74195-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="74195-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74195-112">Not supported.</span></span>  |
|<span data-ttu-id="74195-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74195-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="74195-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74195-114">Not supported.</span></span>  |
|<span data-ttu-id="74195-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74195-115">Application</span></span> | <span data-ttu-id="74195-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="74195-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="74195-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74195-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="74195-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74195-118">Request headers</span></span>
| <span data-ttu-id="74195-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74195-119">Header</span></span>       | <span data-ttu-id="74195-120">Valor</span><span class="sxs-lookup"><span data-stu-id="74195-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74195-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="74195-121">Authorization</span></span>  | <span data-ttu-id="74195-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74195-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="74195-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74195-124">Content-Type</span></span>  | <span data-ttu-id="74195-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74195-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74195-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74195-126">Request body</span></span>
<span data-ttu-id="74195-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="74195-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="74195-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="74195-128">Response</span></span>
<span data-ttu-id="74195-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74195-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74195-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74195-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74195-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74195-131">Request</span></span>
<span data-ttu-id="74195-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74195-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74195-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="74195-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass_1"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```
# <a name="javascript"></a>[<span data-ttu-id="74195-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74195-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74195-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74195-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="74195-136">C#</span><span class="sxs-lookup"><span data-stu-id="74195-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74195-137">Java</span><span class="sxs-lookup"><span data-stu-id="74195-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74195-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="74195-138">Response</span></span>
<span data-ttu-id="74195-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74195-139">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


