---
title: Obter educationCategory
description: Recupere um objeto Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 07c95e1f53ee349955e8937f558faf2940e74938
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427064"
---
# <a name="get-educationcategory"></a><span data-ttu-id="eed52-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="eed52-103">Get educationCategory</span></span>

<span data-ttu-id="eed52-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eed52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eed52-105">Recupere um objeto [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="eed52-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eed52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eed52-106">Permissions</span></span>

<span data-ttu-id="eed52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eed52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed52-109">Permission type</span></span>                        | <span data-ttu-id="eed52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eed52-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="eed52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed52-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eed52-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eed52-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="eed52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eed52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed52-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="eed52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eed52-115">Application</span></span>                            | <span data-ttu-id="eed52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed52-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="eed52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eed52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eed52-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eed52-118">Optional query parameters</span></span>

<span data-ttu-id="eed52-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eed52-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eed52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eed52-120">Request headers</span></span>
| <span data-ttu-id="eed52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eed52-121">Header</span></span>        | <span data-ttu-id="eed52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eed52-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="eed52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eed52-123">Authorization</span></span> | <span data-ttu-id="eed52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eed52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eed52-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eed52-126">Request body</span></span>

<span data-ttu-id="eed52-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eed52-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eed52-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed52-128">Response</span></span>

<span data-ttu-id="eed52-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eed52-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed52-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed52-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eed52-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed52-131">Request</span></span>

<span data-ttu-id="eed52-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eed52-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="eed52-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed52-133">Response</span></span>

<span data-ttu-id="eed52-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eed52-134">The following is an example of the response.</span></span> 

><span data-ttu-id="eed52-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eed52-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
