---
title: Listar usuários
description: Recupera uma lista de objetos de usuário.
author: dkershaw10
ms.openlocfilehash: ad7feaa1d694f3ae44b125f67e5e72b78b3089f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335165"
---
# <a name="list-users"></a><span data-ttu-id="af2a0-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="af2a0-103">List users</span></span>

<span data-ttu-id="af2a0-104">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="af2a0-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="af2a0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af2a0-105">Permissions</span></span>

<span data-ttu-id="af2a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af2a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af2a0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af2a0-108">Permission type</span></span>      | <span data-ttu-id="af2a0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af2a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af2a0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af2a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af2a0-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af2a0-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af2a0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af2a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af2a0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af2a0-113">Not supported.</span></span>    |
|<span data-ttu-id="af2a0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af2a0-114">Application</span></span> | <span data-ttu-id="af2a0-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af2a0-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af2a0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af2a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af2a0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af2a0-117">Optional query parameters</span></span>

<span data-ttu-id="af2a0-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af2a0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="af2a0-119">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="af2a0-119">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="af2a0-120">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="af2a0-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="af2a0-121">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="af2a0-121">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="af2a0-p103">Observação: Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário. As seguintes propriedades só terão suporte na [recuperação de um único usuário](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="af2a0-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="af2a0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a0-124">Request headers</span></span>

| <span data-ttu-id="af2a0-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af2a0-125">Header</span></span>        | <span data-ttu-id="af2a0-126">Valor</span><span class="sxs-lookup"><span data-stu-id="af2a0-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="af2a0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="af2a0-127">Authorization</span></span> | <span data-ttu-id="af2a0-128">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="af2a0-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="af2a0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af2a0-129">Content-Type</span></span>  | <span data-ttu-id="af2a0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="af2a0-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="af2a0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a0-131">Request body</span></span>

<span data-ttu-id="af2a0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af2a0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af2a0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2a0-133">Response</span></span>

<span data-ttu-id="af2a0-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af2a0-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af2a0-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af2a0-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="af2a0-136">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="af2a0-136">Example 1: Standard users request</span></span>

<span data-ttu-id="af2a0-137">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="af2a0-137">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="af2a0-138">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="af2a0-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="af2a0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a0-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="af2a0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2a0-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="af2a0-141">Exemplo 2: Solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="af2a0-141">Example 2: Users request using $select</span></span>

<span data-ttu-id="af2a0-142">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="af2a0-142">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="af2a0-143">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="af2a0-143">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="af2a0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a0-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="af2a0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2a0-145">Response</span></span>

<span data-ttu-id="af2a0-146">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af2a0-146">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
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
