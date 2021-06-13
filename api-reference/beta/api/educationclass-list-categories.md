---
title: Listar assignmentCategories
description: Recupere uma lista de objetos de categoria.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3f7851e746cb87905768604610cd17d036cc963c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911827"
---
# <a name="list-assignmentcategories"></a><span data-ttu-id="7de03-103">Listar assignmentCategories</span><span class="sxs-lookup"><span data-stu-id="7de03-103">List assignmentCategories</span></span>

<span data-ttu-id="7de03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de03-105">Recupere uma lista de [objetos educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="7de03-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7de03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7de03-106">Permissions</span></span>

<span data-ttu-id="7de03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7de03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7de03-109">Permission type</span></span>                        | <span data-ttu-id="7de03-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7de03-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7de03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7de03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7de03-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7de03-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7de03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7de03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7de03-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="7de03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7de03-115">Application</span></span>                            | <span data-ttu-id="7de03-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7de03-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7de03-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7de03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7de03-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7de03-118">Optional query parameters</span></span>

<span data-ttu-id="7de03-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7de03-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7de03-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7de03-120">Request headers</span></span>

| <span data-ttu-id="7de03-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7de03-121">Header</span></span>        | <span data-ttu-id="7de03-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7de03-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7de03-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7de03-123">Authorization</span></span> | <span data-ttu-id="7de03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7de03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7de03-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7de03-126">Request body</span></span>

<span data-ttu-id="7de03-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7de03-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7de03-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de03-128">Response</span></span>

<span data-ttu-id="7de03-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7de03-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7de03-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7de03-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7de03-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7de03-131">Request</span></span>

<span data-ttu-id="7de03-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7de03-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["4797d052-ebf5-4018-a088-e11adc6b2cbb"],
  "name": "get_class_categories"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="7de03-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de03-133">Response</span></span>

<span data-ttu-id="7de03-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7de03-134">The following is an example of the response.</span></span> 

><span data-ttu-id="7de03-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7de03-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('4797d052-ebf5-4018-a088-e11adc6b2cbb')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
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
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
