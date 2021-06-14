---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 891f08305971ec6f19413bae46451e1c4258d065
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912195"
---
# <a name="get-educationcategory"></a><span data-ttu-id="e846c-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="e846c-103">Get educationCategory</span></span>

<span data-ttu-id="e846c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e846c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e846c-105">Recupere um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e846c-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e846c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e846c-106">Permissions</span></span>

<span data-ttu-id="e846c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e846c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e846c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e846c-109">Permission type</span></span>                        | <span data-ttu-id="e846c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e846c-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e846c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e846c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e846c-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e846c-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e846c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e846c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e846c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e846c-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="e846c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e846c-115">Application</span></span>                            | <span data-ttu-id="e846c-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e846c-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e846c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e846c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e846c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e846c-118">Optional query parameters</span></span>

<span data-ttu-id="e846c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e846c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e846c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e846c-120">Request headers</span></span>
| <span data-ttu-id="e846c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e846c-121">Header</span></span>        | <span data-ttu-id="e846c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e846c-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e846c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e846c-123">Authorization</span></span> | <span data-ttu-id="e846c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e846c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e846c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e846c-126">Request body</span></span>

<span data-ttu-id="e846c-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="e846c-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e846c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e846c-128">Response</span></span>

<span data-ttu-id="e846c-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e846c-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e846c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e846c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e846c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e846c-131">Request</span></span>

<span data-ttu-id="e846c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e846c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["acdefc6b-2dc6-4e71-b1e9-6d9810ab1793"],
  "name": "get_class_category"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/96821157-5efb-4706-8ca2-a90b26c44852
```

### <a name="response"></a><span data-ttu-id="e846c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e846c-133">Response</span></span>

<span data-ttu-id="e846c-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e846c-134">The following is an example of the response.</span></span>

><span data-ttu-id="e846c-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e846c-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "96821157-5efb-4706-8ca2-a90b26c44852"
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