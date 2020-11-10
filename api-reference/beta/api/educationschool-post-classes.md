---
title: Adicionar educationClass a educationSchool
description: Adicione uma aula a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 78ec26374d214243649eed60b1e002ccfc425b22
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955523"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="7ecc4-103">Adicionar educationClass a educationSchool</span><span class="sxs-lookup"><span data-stu-id="7ecc4-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="7ecc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ecc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ecc4-105">Adicione uma aula a uma escola.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-105">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ecc4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ecc4-106">Permissions</span></span>
<span data-ttu-id="7ecc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ecc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ecc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ecc4-109">Permission type</span></span>      | <span data-ttu-id="7ecc4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ecc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ecc4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ecc4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="7ecc4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-112">Not supported.</span></span>  |
|<span data-ttu-id="7ecc4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ecc4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7ecc4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-114">Not supported.</span></span>  |
|<span data-ttu-id="7ecc4-115">Application</span><span class="sxs-lookup"><span data-stu-id="7ecc4-115">Application</span></span> | <span data-ttu-id="7ecc4-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecc4-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7ecc4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ecc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7ecc4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ecc4-118">Request headers</span></span>
| <span data-ttu-id="7ecc4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ecc4-119">Header</span></span>       | <span data-ttu-id="7ecc4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7ecc4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ecc4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ecc4-121">Authorization</span></span>  | <span data-ttu-id="7ecc4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ecc4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ecc4-124">Content-Type</span></span>  | <span data-ttu-id="7ecc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ecc4-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ecc4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ecc4-126">Request body</span></span>
<span data-ttu-id="7ecc4-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="7ecc4-127">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7ecc4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ecc4-128">Response</span></span>
<span data-ttu-id="7ecc4-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ecc4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ecc4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ecc4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ecc4-131">Request</span></span>
<span data-ttu-id="7ecc4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ecc4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ecc4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7ecc4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ecc4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ecc4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ecc4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7ecc4-136">C#</span><span class="sxs-lookup"><span data-stu-id="7ecc4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ecc4-137">Java</span><span class="sxs-lookup"><span data-stu-id="7ecc4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ecc4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ecc4-138">Response</span></span> 
<span data-ttu-id="7ecc4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ecc4-139">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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
  ]
}
-->


