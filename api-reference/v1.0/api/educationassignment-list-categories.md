---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 820068cafa4667e4a1d4ea47b6e25b725e8b63fe
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991069"
---
# <a name="list-categories"></a><span data-ttu-id="df453-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="df453-103">List categories</span></span>

<span data-ttu-id="df453-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df453-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df453-105">Lista todas as categorias associadas a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="df453-105">List all the categories associated with an assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="df453-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df453-106">Permissions</span></span>
<span data-ttu-id="df453-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df453-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df453-109">Permission type</span></span>      | <span data-ttu-id="df453-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df453-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df453-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df453-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="df453-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df453-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="df453-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df453-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df453-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df453-114">Not supported.</span></span>  |
|<span data-ttu-id="df453-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df453-115">Application</span></span> | <span data-ttu-id="df453-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df453-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df453-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df453-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="df453-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df453-118">Optional query parameters</span></span>
<span data-ttu-id="df453-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df453-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df453-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df453-120">Request headers</span></span>
| <span data-ttu-id="df453-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df453-121">Header</span></span>       | <span data-ttu-id="df453-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df453-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df453-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df453-123">Authorization</span></span>  | <span data-ttu-id="df453-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df453-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df453-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df453-126">Request body</span></span>
<span data-ttu-id="df453-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="df453-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df453-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df453-128">Response</span></span>
<span data-ttu-id="df453-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df453-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df453-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df453-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="df453-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df453-131">Request</span></span>
<span data-ttu-id="df453-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df453-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df453-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df453-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_assignment_categories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories
```
# <a name="c"></a>[<span data-ttu-id="df453-134">C#</span><span class="sxs-lookup"><span data-stu-id="df453-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignment-categories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df453-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df453-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignment-categories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df453-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df453-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignment-categories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df453-137">Java</span><span class="sxs-lookup"><span data-stu-id="df453-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignment-categories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df453-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="df453-138">Response</span></span>
<span data-ttu-id="df453-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df453-139">The following is an example of the response.</span></span> 

><span data-ttu-id="df453-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df453-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('a17025d0-62a8-4450-9e6e-db31d8c8feb8')/assignments('1fdf61ee-c129-4960-9b7c-8df159aa64b0')/categories",
    "value": [
        {
            "displayName": "Quizzes",
            "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
