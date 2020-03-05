---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 779c54b7b56e72b6c543d36e1e1a9d0ae190d51a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427568"
---
# <a name="list-categories"></a><span data-ttu-id="9ce00-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="9ce00-103">List categories</span></span>

<span data-ttu-id="9ce00-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9ce00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce00-105">Listar todas as categorias associadas a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="9ce00-105">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ce00-106">Permissions</span></span>
<span data-ttu-id="9ce00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ce00-109">Permission type</span></span>      | <span data-ttu-id="9ce00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ce00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ce00-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ce00-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ce00-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9ce00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ce00-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ce00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ce00-114">Not supported.</span></span>  |
|<span data-ttu-id="9ce00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ce00-115">Application</span></span> | <span data-ttu-id="9ce00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ce00-116">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ce00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ce00-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ce00-118">Optional query parameters</span></span>
<span data-ttu-id="9ce00-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ce00-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ce00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ce00-120">Request headers</span></span>
| <span data-ttu-id="9ce00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ce00-121">Header</span></span>       | <span data-ttu-id="9ce00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ce00-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ce00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ce00-123">Authorization</span></span>  | <span data-ttu-id="9ce00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ce00-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ce00-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ce00-126">Request body</span></span>
<span data-ttu-id="9ce00-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ce00-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9ce00-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ce00-128">Response</span></span>
<span data-ttu-id="9ce00-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ce00-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ce00-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ce00-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ce00-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ce00-131">Request</span></span>
<span data-ttu-id="9ce00-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ce00-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="9ce00-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ce00-133">Response</span></span>
<span data-ttu-id="9ce00-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ce00-134">The following is an example of the response.</span></span> 

><span data-ttu-id="9ce00-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9ce00-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ce00-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ce00-136">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
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
