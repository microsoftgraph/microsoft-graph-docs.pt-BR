---
title: Obter educationCategory
description: Recupere um objeto Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c88e8ae48aade64fb5f219008e277063dae46f1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810873"
---
# <a name="get-educationcategory"></a><span data-ttu-id="85fec-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="85fec-103">Get educationCategory</span></span>

<span data-ttu-id="85fec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85fec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85fec-105">Recupere um objeto [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="85fec-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85fec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85fec-106">Permissions</span></span>

<span data-ttu-id="85fec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85fec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85fec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85fec-109">Permission type</span></span>                        | <span data-ttu-id="85fec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85fec-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="85fec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85fec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85fec-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85fec-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="85fec-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85fec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85fec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85fec-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="85fec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85fec-115">Application</span></span>                            | <span data-ttu-id="85fec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85fec-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="85fec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85fec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85fec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85fec-118">Optional query parameters</span></span>

<span data-ttu-id="85fec-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85fec-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85fec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85fec-120">Request headers</span></span>
| <span data-ttu-id="85fec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85fec-121">Header</span></span>        | <span data-ttu-id="85fec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85fec-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="85fec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85fec-123">Authorization</span></span> | <span data-ttu-id="85fec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85fec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85fec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85fec-126">Request body</span></span>

<span data-ttu-id="85fec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85fec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85fec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fec-128">Response</span></span>

<span data-ttu-id="85fec-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85fec-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85fec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85fec-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85fec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85fec-131">Request</span></span>

<span data-ttu-id="85fec-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85fec-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="85fec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fec-133">Response</span></span>

<span data-ttu-id="85fec-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85fec-134">The following is an example of the response.</span></span>

><span data-ttu-id="85fec-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85fec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
