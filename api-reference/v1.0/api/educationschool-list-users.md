---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1889dfd19ab5ef461cccff5a2dc0103fce79cb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550270"
---
# <a name="list-educationusers"></a><span data-ttu-id="e6165-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="e6165-103">List educationUsers</span></span>

<span data-ttu-id="e6165-104">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="e6165-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6165-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6165-105">Permissions</span></span>
<span data-ttu-id="e6165-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6165-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6165-108">Permission type</span></span>      | <span data-ttu-id="e6165-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6165-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6165-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6165-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6165-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6165-111">Not supported.</span></span>  |
|<span data-ttu-id="e6165-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6165-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6165-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6165-113">Not supported.</span></span>  |
|<span data-ttu-id="e6165-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6165-114">Application</span></span> | <span data-ttu-id="e6165-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6165-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e6165-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6165-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6165-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e6165-117">Optional query parameters</span></span>
<span data-ttu-id="e6165-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e6165-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6165-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6165-119">Request headers</span></span>
| <span data-ttu-id="e6165-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6165-120">Header</span></span>       | <span data-ttu-id="e6165-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e6165-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6165-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6165-122">Authorization</span></span>  | <span data-ttu-id="e6165-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6165-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6165-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6165-125">Request body</span></span>
<span data-ttu-id="e6165-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6165-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e6165-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6165-127">Response</span></span>
<span data-ttu-id="e6165-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6165-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6165-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6165-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6165-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6165-130">Request</span></span>
<span data-ttu-id="e6165-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6165-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
##### <a name="response"></a><span data-ttu-id="e6165-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6165-132">Response</span></span>
<span data-ttu-id="e6165-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6165-133">The following is an example of the response.</span></span> 

><span data-ttu-id="e6165-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6165-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
