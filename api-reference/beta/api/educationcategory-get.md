---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fed72875c029c2080af7f8e2133a2f2a6d94b3ba
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061781"
---
# <a name="get-educationcategory"></a><span data-ttu-id="07b13-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="07b13-103">Get educationCategory</span></span>

<span data-ttu-id="07b13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07b13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07b13-105">Recupere um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="07b13-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="07b13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07b13-106">Permissions</span></span>

<span data-ttu-id="07b13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07b13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07b13-109">Permission type</span></span>                        | <span data-ttu-id="07b13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07b13-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="07b13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07b13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="07b13-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07b13-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="07b13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07b13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07b13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07b13-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="07b13-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="07b13-115">Application\*</span></span>                           | <span data-ttu-id="07b13-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07b13-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="07b13-117">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="07b13-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="07b13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07b13-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07b13-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07b13-119">Optional query parameters</span></span>

<span data-ttu-id="07b13-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07b13-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07b13-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07b13-121">Request headers</span></span>
| <span data-ttu-id="07b13-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07b13-122">Header</span></span>        | <span data-ttu-id="07b13-123">Valor</span><span class="sxs-lookup"><span data-stu-id="07b13-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="07b13-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07b13-124">Authorization</span></span> | <span data-ttu-id="07b13-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07b13-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07b13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07b13-127">Request body</span></span>

<span data-ttu-id="07b13-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07b13-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07b13-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b13-129">Response</span></span>

<span data-ttu-id="07b13-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07b13-130">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07b13-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07b13-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="07b13-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07b13-132">Request</span></span>

<span data-ttu-id="07b13-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07b13-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="07b13-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b13-134">Response</span></span>

<span data-ttu-id="07b13-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07b13-135">The following is an example of the response.</span></span>

><span data-ttu-id="07b13-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="07b13-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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