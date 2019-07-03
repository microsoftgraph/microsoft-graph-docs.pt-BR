---
title: Adicionar professor
description: Adicione um professor a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 090f613499fe693c2d1c9000ee3eb963ebae6aa6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449894"
---
# <a name="add-teacher"></a><span data-ttu-id="808e8-103">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="808e8-103">Add teacher</span></span>

<span data-ttu-id="808e8-104">Adicione um professor a uma aula.</span><span class="sxs-lookup"><span data-stu-id="808e8-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="808e8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="808e8-105">Permissions</span></span>
<span data-ttu-id="808e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="808e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="808e8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="808e8-108">Permission type</span></span>      | <span data-ttu-id="808e8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="808e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="808e8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="808e8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="808e8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="808e8-111">Not supported.</span></span>  |
|<span data-ttu-id="808e8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="808e8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="808e8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="808e8-113">Not supported.</span></span>  |
|<span data-ttu-id="808e8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="808e8-114">Application</span></span> | <span data-ttu-id="808e8-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="808e8-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="808e8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="808e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="808e8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-117">Request headers</span></span>
| <span data-ttu-id="808e8-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="808e8-118">Header</span></span>       | <span data-ttu-id="808e8-119">Valor</span><span class="sxs-lookup"><span data-stu-id="808e8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="808e8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="808e8-120">Authorization</span></span>  | <span data-ttu-id="808e8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="808e8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="808e8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="808e8-123">Content-Type</span></span>  | <span data-ttu-id="808e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="808e8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="808e8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-125">Request body</span></span>
<span data-ttu-id="808e8-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="808e8-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="808e8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="808e8-127">Response</span></span>
<span data-ttu-id="808e8-128">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="808e8-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="808e8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="808e8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="808e8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-130">Request</span></span>
<span data-ttu-id="808e8-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="808e8-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="808e8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="808e8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="808e8-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="808e8-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="808e8-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="808e8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="808e8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="808e8-135">Response</span></span>
<span data-ttu-id="808e8-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="808e8-136">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="808e8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="808e8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
