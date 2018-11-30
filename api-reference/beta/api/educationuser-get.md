---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
ms.openlocfilehash: e40b4bfea7daa1d6df1b5d06b9a8e67407647b28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033013"
---
# <a name="get-educationuser"></a><span data-ttu-id="2bdcb-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="2bdcb-103">Get educationUser</span></span>

> <span data-ttu-id="2bdcb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bdcb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bdcb-106">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-106">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bdcb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2bdcb-107">Permissions</span></span>
<span data-ttu-id="2bdcb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdcb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bdcb-110">Permission type</span></span>      | <span data-ttu-id="2bdcb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bdcb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bdcb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bdcb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2bdcb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2bdcb-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2bdcb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bdcb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2bdcb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-115">Not supported.</span></span>  |
|<span data-ttu-id="2bdcb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bdcb-116">Application</span></span> | <span data-ttu-id="2bdcb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdcb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="2bdcb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdcb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bdcb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bdcb-119">Optional query parameters</span></span>
<span data-ttu-id="2bdcb-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bdcb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcb-121">Request headers</span></span>
| <span data-ttu-id="2bdcb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bdcb-122">Header</span></span>       | <span data-ttu-id="2bdcb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2bdcb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2bdcb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bdcb-124">Authorization</span></span>  | <span data-ttu-id="2bdcb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bdcb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcb-127">Request body</span></span>
<span data-ttu-id="2bdcb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2bdcb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdcb-129">Response</span></span>
<span data-ttu-id="2bdcb-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-130">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bdcb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bdcb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bdcb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcb-132">Request</span></span>
<span data-ttu-id="2bdcb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="2bdcb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdcb-134">Response</span></span>
<span data-ttu-id="2bdcb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2bdcb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bdcb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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