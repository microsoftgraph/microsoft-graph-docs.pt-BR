---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: fed061fd5afc867126c7cc70ee702e937a8eba4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833576"
---
# <a name="list-educationusers"></a><span data-ttu-id="f1a95-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="f1a95-103">List educationUsers</span></span>

> <span data-ttu-id="f1a95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1a95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1a95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1a95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1a95-106">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="f1a95-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a95-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1a95-107">Permissions</span></span>
<span data-ttu-id="f1a95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1a95-110">Permission type</span></span>      | <span data-ttu-id="f1a95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1a95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1a95-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1a95-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1a95-113">Not supported.</span></span>  |
|<span data-ttu-id="f1a95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1a95-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1a95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1a95-115">Not supported.</span></span>  |
|<span data-ttu-id="f1a95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1a95-116">Application</span></span> | <span data-ttu-id="f1a95-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a95-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f1a95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1a95-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1a95-119">Optional query parameters</span></span>
<span data-ttu-id="f1a95-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a95-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1a95-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a95-121">Request headers</span></span>
| <span data-ttu-id="f1a95-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1a95-122">Header</span></span>       | <span data-ttu-id="f1a95-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1a95-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1a95-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1a95-124">Authorization</span></span>  | <span data-ttu-id="f1a95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1a95-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1a95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a95-127">Request body</span></span>
<span data-ttu-id="f1a95-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1a95-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f1a95-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a95-129">Response</span></span>
<span data-ttu-id="f1a95-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a95-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1a95-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1a95-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a95-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a95-132">Request</span></span>
<span data-ttu-id="f1a95-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1a95-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="f1a95-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a95-134">Response</span></span>
<span data-ttu-id="f1a95-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a95-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f1a95-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1a95-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
