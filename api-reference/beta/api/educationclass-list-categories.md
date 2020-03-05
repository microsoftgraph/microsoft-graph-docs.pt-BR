---
title: Listar educationCategories
description: Recupere uma lista de objetos Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f647c0b5241dc7ab98d0fda5f3ccce8233a6b557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426693"
---
# <a name="list-educationcategories"></a><span data-ttu-id="24650-103">Listar educationCategories</span><span class="sxs-lookup"><span data-stu-id="24650-103">List educationCategories</span></span>

<span data-ttu-id="24650-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24650-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24650-105">Recupere uma lista de objetos [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="24650-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="24650-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24650-106">Permissions</span></span>

<span data-ttu-id="24650-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24650-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24650-109">Permission type</span></span>                        | <span data-ttu-id="24650-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24650-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="24650-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24650-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24650-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24650-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="24650-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24650-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24650-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24650-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="24650-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24650-115">Application</span></span>                            | <span data-ttu-id="24650-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24650-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="24650-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24650-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24650-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24650-118">Optional query parameters</span></span>

<span data-ttu-id="24650-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24650-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24650-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24650-120">Request headers</span></span>

| <span data-ttu-id="24650-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24650-121">Header</span></span>        | <span data-ttu-id="24650-122">Valor</span><span class="sxs-lookup"><span data-stu-id="24650-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="24650-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24650-123">Authorization</span></span> | <span data-ttu-id="24650-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24650-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24650-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24650-126">Request body</span></span>

<span data-ttu-id="24650-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24650-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24650-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24650-128">Response</span></span>

<span data-ttu-id="24650-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24650-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24650-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24650-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="24650-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24650-131">Request</span></span>

<span data-ttu-id="24650-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24650-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="24650-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="24650-133">Response</span></span>

<span data-ttu-id="24650-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24650-134">The following is an example of the response.</span></span> 

><span data-ttu-id="24650-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24650-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
