---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
ms.openlocfilehash: 24bcf5b680cdb29684f9647bd3e9632b896594a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035312"
---
# <a name="list-educationusers"></a><span data-ttu-id="01a6d-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="01a6d-103">List educationUsers</span></span>

> <span data-ttu-id="01a6d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01a6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01a6d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01a6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01a6d-106">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="01a6d-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="01a6d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01a6d-107">Permissions</span></span>
<span data-ttu-id="01a6d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a6d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01a6d-110">Permission type</span></span>      | <span data-ttu-id="01a6d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01a6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a6d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01a6d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="01a6d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a6d-113">Not supported.</span></span>  |
|<span data-ttu-id="01a6d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01a6d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="01a6d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a6d-115">Not supported.</span></span>  |
|<span data-ttu-id="01a6d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01a6d-116">Application</span></span> | <span data-ttu-id="01a6d-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a6d-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="01a6d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01a6d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01a6d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01a6d-119">Optional query parameters</span></span>
<span data-ttu-id="01a6d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01a6d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01a6d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01a6d-121">Request headers</span></span>
| <span data-ttu-id="01a6d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01a6d-122">Header</span></span>       | <span data-ttu-id="01a6d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="01a6d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01a6d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="01a6d-124">Authorization</span></span>  | <span data-ttu-id="01a6d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01a6d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01a6d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01a6d-127">Request body</span></span>
<span data-ttu-id="01a6d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01a6d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="01a6d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a6d-129">Response</span></span>
<span data-ttu-id="01a6d-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01a6d-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01a6d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01a6d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01a6d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01a6d-132">Request</span></span>
<span data-ttu-id="01a6d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01a6d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="01a6d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a6d-134">Response</span></span>
<span data-ttu-id="01a6d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01a6d-135">The following is an example of the response.</span></span> 

><span data-ttu-id="01a6d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01a6d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
