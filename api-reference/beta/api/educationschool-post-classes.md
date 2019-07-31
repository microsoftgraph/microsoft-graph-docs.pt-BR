---
title: Adicionar educationClass a educationSchool
description: Adicione uma aula a uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b904ed3697dbe1f804e63619f135f96142481ce9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955142"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="c3347-103">Adicionar educationClass a educationSchool</span><span class="sxs-lookup"><span data-stu-id="c3347-103">Add educationClass to educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3347-104">Adicione uma aula a uma escola.</span><span class="sxs-lookup"><span data-stu-id="c3347-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3347-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3347-105">Permissions</span></span>
<span data-ttu-id="c3347-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3347-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3347-108">Permission type</span></span>      | <span data-ttu-id="c3347-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3347-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3347-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3347-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c3347-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3347-111">Not supported.</span></span>  |
|<span data-ttu-id="c3347-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3347-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c3347-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3347-113">Not supported.</span></span>  |
|<span data-ttu-id="c3347-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3347-114">Application</span></span> | <span data-ttu-id="c3347-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3347-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3347-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3347-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c3347-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3347-117">Request headers</span></span>
| <span data-ttu-id="c3347-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3347-118">Header</span></span>       | <span data-ttu-id="c3347-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c3347-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3347-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3347-120">Authorization</span></span>  | <span data-ttu-id="c3347-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3347-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c3347-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3347-123">Content-Type</span></span>  | <span data-ttu-id="c3347-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3347-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3347-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3347-125">Request body</span></span>
<span data-ttu-id="c3347-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="c3347-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c3347-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3347-127">Response</span></span>
<span data-ttu-id="c3347-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3347-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3347-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3347-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3347-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3347-130">Request</span></span>
<span data-ttu-id="c3347-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3347-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3347-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3347-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3347-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3347-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3347-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3347-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="c3347-135">C#</span><span class="sxs-lookup"><span data-stu-id="c3347-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3347-136">Java</span><span class="sxs-lookup"><span data-stu-id="c3347-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c3347-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3347-137">Response</span></span> 
<span data-ttu-id="c3347-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3347-138">The following is an example of the response.</span></span> 

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
