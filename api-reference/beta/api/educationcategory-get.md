---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1c7dc80eb2e23dbf1fc09f9b906770b3b3a0fb47
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044082"
---
# <a name="get-educationcategory"></a><span data-ttu-id="cb753-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="cb753-103">Get educationCategory</span></span>

<span data-ttu-id="cb753-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb753-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb753-105">Recupere um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="cb753-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb753-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb753-106">Permissions</span></span>

<span data-ttu-id="cb753-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb753-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb753-109">Permission type</span></span>                        | <span data-ttu-id="cb753-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb753-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cb753-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb753-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb753-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb753-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="cb753-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb753-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb753-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb753-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="cb753-115">Application</span><span class="sxs-lookup"><span data-stu-id="cb753-115">Application</span></span>                            | <span data-ttu-id="cb753-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb753-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb753-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb753-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb753-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb753-118">Optional query parameters</span></span>

<span data-ttu-id="cb753-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb753-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb753-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb753-120">Request headers</span></span>
| <span data-ttu-id="cb753-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb753-121">Header</span></span>        | <span data-ttu-id="cb753-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb753-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cb753-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb753-123">Authorization</span></span> | <span data-ttu-id="cb753-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb753-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb753-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb753-126">Request body</span></span>

<span data-ttu-id="cb753-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb753-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb753-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb753-128">Response</span></span>

<span data-ttu-id="cb753-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb753-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb753-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb753-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cb753-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb753-131">Request</span></span>

<span data-ttu-id="cb753-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb753-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="cb753-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb753-133">Response</span></span>

<span data-ttu-id="cb753-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb753-134">The following is an example of the response.</span></span>

><span data-ttu-id="cb753-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb753-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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
}
```

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