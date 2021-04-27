---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 319d2d09ec25a95bfaacd13d87a10f390ee10777
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044386"
---
# <a name="list-categories"></a><span data-ttu-id="6ce30-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="6ce30-103">List categories</span></span>

<span data-ttu-id="6ce30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ce30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ce30-105">Listar todas as categorias associadas a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="6ce30-105">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ce30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ce30-106">Permissions</span></span>
<span data-ttu-id="6ce30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ce30-109">Permission type</span></span>      | <span data-ttu-id="6ce30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ce30-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ce30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ce30-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6ce30-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ce30-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6ce30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ce30-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6ce30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ce30-114">Not supported.</span></span>  |
|<span data-ttu-id="6ce30-115">Application</span><span class="sxs-lookup"><span data-stu-id="6ce30-115">Application</span></span> | <span data-ttu-id="6ce30-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ce30-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6ce30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce30-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ce30-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ce30-118">Optional query parameters</span></span>
<span data-ttu-id="6ce30-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ce30-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ce30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce30-120">Request headers</span></span>
| <span data-ttu-id="6ce30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ce30-121">Header</span></span>       | <span data-ttu-id="6ce30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ce30-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ce30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ce30-123">Authorization</span></span>  | <span data-ttu-id="6ce30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ce30-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ce30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce30-126">Request body</span></span>
<span data-ttu-id="6ce30-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ce30-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6ce30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce30-128">Response</span></span>
<span data-ttu-id="6ce30-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ce30-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ce30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ce30-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ce30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce30-131">Request</span></span>
<span data-ttu-id="6ce30-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ce30-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="6ce30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce30-133">Response</span></span>
<span data-ttu-id="6ce30-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ce30-134">The following is an example of the response.</span></span> 

><span data-ttu-id="6ce30-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ce30-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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