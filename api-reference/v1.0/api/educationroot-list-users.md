---
title: Listar usuários
description: Recupera uma lista de objetos de usuário. Esses objetos de usuário incluirão propriedades específicas de educação.
ms.openlocfilehash: 8b0c0fb88323700fe2fdb0d7236f0a6e1183ce15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004488"
---
# <a name="list-users"></a><span data-ttu-id="12b46-104">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="12b46-104">List users</span></span>

<span data-ttu-id="12b46-105">Recupera uma lista de objetos de usuário.</span><span class="sxs-lookup"><span data-stu-id="12b46-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="12b46-106">Esses objetos de usuário incluirão propriedades específicas de educação.</span><span class="sxs-lookup"><span data-stu-id="12b46-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="12b46-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="12b46-107">Permissions</span></span>
<span data-ttu-id="12b46-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12b46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b46-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12b46-110">Permission type</span></span>      | <span data-ttu-id="12b46-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12b46-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12b46-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12b46-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="12b46-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12b46-113">Not supported.</span></span>  |
|<span data-ttu-id="12b46-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12b46-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="12b46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12b46-115">Not supported.</span></span>  |
|<span data-ttu-id="12b46-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12b46-116">Application</span></span> | <span data-ttu-id="12b46-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b46-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="12b46-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12b46-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12b46-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12b46-119">Optional query parameters</span></span>
<span data-ttu-id="12b46-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12b46-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12b46-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12b46-121">Request headers</span></span>
| <span data-ttu-id="12b46-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12b46-122">Header</span></span>       | <span data-ttu-id="12b46-123">Valor</span><span class="sxs-lookup"><span data-stu-id="12b46-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12b46-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12b46-124">Authorization</span></span>  | <span data-ttu-id="12b46-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12b46-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12b46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12b46-127">Request body</span></span>
<span data-ttu-id="12b46-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12b46-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="12b46-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="12b46-129">Response</span></span>
<span data-ttu-id="12b46-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12b46-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12b46-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12b46-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12b46-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12b46-132">Request</span></span>
<span data-ttu-id="12b46-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12b46-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="12b46-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="12b46-134">Response</span></span>
<span data-ttu-id="12b46-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12b46-135">The following is an example of the response.</span></span> 

><span data-ttu-id="12b46-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12b46-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
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
