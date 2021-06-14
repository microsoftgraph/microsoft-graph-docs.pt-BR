---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15e6be29aa4f39772559506043d1de5f5c6bae35
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912163"
---
# <a name="list-categories"></a><span data-ttu-id="bed4b-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="bed4b-103">List categories</span></span>

<span data-ttu-id="bed4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bed4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bed4b-105">Lista todas as categorias associadas a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="bed4b-105">List all the categories associated with an assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="bed4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bed4b-106">Permissions</span></span>
<span data-ttu-id="bed4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bed4b-109">Permission type</span></span>      | <span data-ttu-id="bed4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bed4b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bed4b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bed4b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bed4b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bed4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bed4b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bed4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bed4b-114">Not supported.</span></span>  |
|<span data-ttu-id="bed4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bed4b-115">Application</span></span> | <span data-ttu-id="bed4b-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bed4b-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bed4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bed4b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bed4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bed4b-118">Optional query parameters</span></span>
<span data-ttu-id="bed4b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bed4b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bed4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bed4b-120">Request headers</span></span>
| <span data-ttu-id="bed4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bed4b-121">Header</span></span>       | <span data-ttu-id="bed4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bed4b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bed4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bed4b-123">Authorization</span></span>  | <span data-ttu-id="bed4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bed4b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bed4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bed4b-126">Request body</span></span>
<span data-ttu-id="bed4b-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="bed4b-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bed4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed4b-128">Response</span></span>
<span data-ttu-id="bed4b-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bed4b-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed4b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bed4b-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="bed4b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bed4b-131">Request</span></span>
<span data-ttu-id="bed4b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bed4b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_assignment_categories"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories
```

### <a name="response"></a><span data-ttu-id="bed4b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed4b-133">Response</span></span>
<span data-ttu-id="bed4b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bed4b-134">The following is an example of the response.</span></span> 

><span data-ttu-id="bed4b-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bed4b-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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
