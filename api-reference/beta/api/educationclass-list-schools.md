---
title: Listar escolas
description: Recupere uma lista de escolas nas quais a aula é ministrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8e79825a4c31ef6c6d4910dd3826d24176d17c71
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457764"
---
# <a name="list-schools"></a><span data-ttu-id="f5c83-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="f5c83-103">List schools</span></span>

<span data-ttu-id="f5c83-104">Recupere uma lista de escolas nas quais a aula é ministrada.</span><span class="sxs-lookup"><span data-stu-id="f5c83-104">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5c83-105">Permissions</span></span>
<span data-ttu-id="f5c83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5c83-108">Permission type</span></span>      | <span data-ttu-id="f5c83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5c83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c83-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c83-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5c83-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f5c83-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="f5c83-112">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5c83-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f5c83-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f5c83-113">Not supported</span></span>  |
|<span data-ttu-id="f5c83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c83-114">Application</span></span> | <span data-ttu-id="f5c83-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5c83-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f5c83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5c83-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5c83-117">Optional query parameters</span></span>
<span data-ttu-id="f5c83-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c83-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5c83-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c83-119">Request headers</span></span>
| <span data-ttu-id="f5c83-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5c83-120">Header</span></span>       | <span data-ttu-id="f5c83-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5c83-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5c83-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c83-122">Authorization</span></span>  | <span data-ttu-id="f5c83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c83-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="f5c83-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c83-125">Request body</span></span>
<span data-ttu-id="f5c83-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5c83-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f5c83-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c83-127">Response</span></span>
<span data-ttu-id="f5c83-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c83-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5c83-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5c83-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5c83-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c83-130">Request</span></span>
<span data-ttu-id="f5c83-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c83-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/schools
```
##### <a name="response"></a><span data-ttu-id="f5c83-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c83-132">Response</span></span>
<span data-ttu-id="f5c83-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c83-133">The following is an example of the response.</span></span> 

><span data-ttu-id="f5c83-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5c83-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
