---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: adcdc634129dc2d4e58941a86d52989e774535e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956476"
---
# <a name="get-educationuser"></a><span data-ttu-id="5b6d0-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="5b6d0-103">Get educationUser</span></span>

> <span data-ttu-id="5b6d0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b6d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b6d0-106">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-106">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6d0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b6d0-107">Permissions</span></span>
<span data-ttu-id="5b6d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6d0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b6d0-110">Permission type</span></span>      | <span data-ttu-id="5b6d0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b6d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6d0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b6d0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5b6d0-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5b6d0-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="5b6d0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b6d0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5b6d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-115">Not supported.</span></span>  |
|<span data-ttu-id="5b6d0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b6d0-116">Application</span></span> | <span data-ttu-id="5b6d0-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6d0-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="5b6d0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b6d0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b6d0-119">Optional query parameters</span></span>
<span data-ttu-id="5b6d0-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b6d0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6d0-121">Request headers</span></span>
| <span data-ttu-id="5b6d0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b6d0-122">Header</span></span>       | <span data-ttu-id="5b6d0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5b6d0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b6d0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b6d0-124">Authorization</span></span>  | <span data-ttu-id="5b6d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b6d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6d0-127">Request body</span></span>
<span data-ttu-id="5b6d0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5b6d0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6d0-129">Response</span></span>
<span data-ttu-id="5b6d0-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-130">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b6d0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b6d0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b6d0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6d0-132">Request</span></span>
<span data-ttu-id="5b6d0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="5b6d0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6d0-134">Response</span></span>
<span data-ttu-id="5b6d0-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5b6d0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
