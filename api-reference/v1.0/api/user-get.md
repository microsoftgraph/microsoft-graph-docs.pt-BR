---
title: Obter um usuário
description: Recupere as propriedades e os relacionamentos do objeto user.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 8b21e45c5b6e86a539a2056859a0afa007614fcf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886209"
---
# <a name="get-a-user"></a><span data-ttu-id="c02f6-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="c02f6-103">Get a user</span></span>

<span data-ttu-id="c02f6-104">Recupere as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="c02f6-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="c02f6-p101">Observação: obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c02f6-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c02f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c02f6-107">Permissions</span></span>
<span data-ttu-id="c02f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c02f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c02f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c02f6-110">Permission type</span></span>      | <span data-ttu-id="c02f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c02f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c02f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c02f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c02f6-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c02f6-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c02f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c02f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c02f6-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c02f6-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="c02f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c02f6-116">Application</span></span> | <span data-ttu-id="c02f6-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c02f6-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c02f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c02f6-118">HTTP request</span></span>
<span data-ttu-id="c02f6-119">Para um usuário específico:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="c02f6-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="c02f6-120">Para o usuário entrou no:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="c02f6-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c02f6-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c02f6-121">Optional query parameters</span></span>
<span data-ttu-id="c02f6-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c02f6-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c02f6-123">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="c02f6-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="c02f6-124">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c02f6-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="c02f6-125">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="c02f6-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="c02f6-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c02f6-126">Request headers</span></span>
| <span data-ttu-id="c02f6-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c02f6-127">Header</span></span>       | <span data-ttu-id="c02f6-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c02f6-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c02f6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c02f6-129">Authorization</span></span>  | <span data-ttu-id="c02f6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c02f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c02f6-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c02f6-132">Content-Type</span></span>   | <span data-ttu-id="c02f6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c02f6-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c02f6-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c02f6-134">Request body</span></span>
<span data-ttu-id="c02f6-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c02f6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c02f6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02f6-136">Response</span></span>

<span data-ttu-id="c02f6-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c02f6-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c02f6-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c02f6-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="c02f6-139">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="c02f6-139">Example 1: Standard users request</span></span>

<span data-ttu-id="c02f6-140">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="c02f6-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="c02f6-141">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="c02f6-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="c02f6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02f6-142">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="c02f6-143">Exemplo 2: solicitação de usuário conectado</span><span class="sxs-lookup"><span data-stu-id="c02f6-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="c02f6-144">Você pode obter as informações do usuário para o usuário conectado, substituindo `/users/{id | userPrincipalName}` por `/me`.</span><span class="sxs-lookup"><span data-stu-id="c02f6-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="c02f6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c02f6-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="c02f6-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02f6-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="c02f6-147">Exemplo 3: solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="c02f6-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="c02f6-148">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c02f6-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="c02f6-149">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="c02f6-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="c02f6-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c02f6-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="c02f6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02f6-151">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
