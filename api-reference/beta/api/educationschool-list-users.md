---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c7e58ac5a1618a97e81fc4377e929bfeae67135a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935098"
---
# <a name="list-educationusers"></a><span data-ttu-id="efead-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="efead-103">List educationUsers</span></span>

> <span data-ttu-id="efead-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="efead-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efead-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efead-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efead-106">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="efead-106">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="efead-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="efead-107">Permissions</span></span>
<span data-ttu-id="efead-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efead-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efead-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efead-110">Permission type</span></span>      | <span data-ttu-id="efead-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efead-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efead-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efead-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="efead-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efead-113">Not supported.</span></span>  |
|<span data-ttu-id="efead-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efead-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="efead-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efead-115">Not supported.</span></span>  |
|<span data-ttu-id="efead-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efead-116">Application</span></span> | <span data-ttu-id="efead-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efead-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="efead-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efead-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efead-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="efead-119">Optional query parameters</span></span>
<span data-ttu-id="efead-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="efead-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efead-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efead-121">Request headers</span></span>
| <span data-ttu-id="efead-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efead-122">Header</span></span>       | <span data-ttu-id="efead-123">Valor</span><span class="sxs-lookup"><span data-stu-id="efead-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="efead-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="efead-124">Authorization</span></span>  | <span data-ttu-id="efead-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efead-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efead-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efead-127">Request body</span></span>
<span data-ttu-id="efead-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efead-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="efead-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="efead-129">Response</span></span>
<span data-ttu-id="efead-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efead-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efead-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efead-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efead-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efead-132">Request</span></span>
<span data-ttu-id="efead-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="efead-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="efead-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="efead-134">Response</span></span>
<span data-ttu-id="efead-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="efead-135">The following is an example of the response.</span></span> 

><span data-ttu-id="efead-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efead-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
