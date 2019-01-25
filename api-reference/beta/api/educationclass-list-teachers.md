---
title: Listar professores
description: Recupere uma lista de professores de uma aula. Os tokens delegados devem ser membros da aula para obterem a lista de professores.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 16f402ba6892ae02d98902688e1cf3b04be316d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514520"
---
# <a name="list-teachers"></a><span data-ttu-id="b9770-104">Listar professores</span><span class="sxs-lookup"><span data-stu-id="b9770-104">List teachers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9770-105">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b9770-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="b9770-106">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="b9770-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9770-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9770-107">Permissions</span></span>
<span data-ttu-id="b9770-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9770-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9770-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9770-110">Permission type</span></span>      | <span data-ttu-id="b9770-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9770-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9770-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9770-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9770-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b9770-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b9770-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9770-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="b9770-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9770-115">Not supported.</span></span>  |
|<span data-ttu-id="b9770-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9770-116">Application</span></span> | <span data-ttu-id="b9770-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9770-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9770-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9770-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9770-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9770-119">Optional query parameters</span></span>
<span data-ttu-id="b9770-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9770-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9770-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9770-121">Request headers</span></span>
| <span data-ttu-id="b9770-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9770-122">Header</span></span>       | <span data-ttu-id="b9770-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b9770-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9770-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9770-124">Authorization</span></span>  | <span data-ttu-id="b9770-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9770-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9770-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9770-127">Request body</span></span>
<span data-ttu-id="b9770-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9770-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9770-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9770-129">Response</span></span>
<span data-ttu-id="b9770-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9770-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9770-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9770-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9770-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9770-132">Request</span></span>
<span data-ttu-id="b9770-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9770-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="b9770-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9770-134">Response</span></span>
<span data-ttu-id="b9770-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9770-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b9770-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9770-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-teachers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
