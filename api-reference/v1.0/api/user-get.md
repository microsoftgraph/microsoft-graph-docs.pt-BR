---
title: Obter um usuário
description: Recupere as propriedades e os relacionamentos do objeto user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc408abf60ad42f564c4c36a37151db122ad573d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984147"
---
# <a name="get-a-user"></a><span data-ttu-id="a41c3-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="a41c3-103">Get a user</span></span>

<span data-ttu-id="a41c3-104">Recupere as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="a41c3-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="a41c3-p101">Observação: obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a41c3-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a41c3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a41c3-107">Permissions</span></span>
<span data-ttu-id="a41c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a41c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a41c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a41c3-110">Permission type</span></span>      | <span data-ttu-id="a41c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a41c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a41c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a41c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a41c3-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a41c3-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a41c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a41c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a41c3-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a41c3-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="a41c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a41c3-116">Application</span></span> | <span data-ttu-id="a41c3-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a41c3-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a41c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a41c3-118">HTTP request</span></span>
<span data-ttu-id="a41c3-119">Para um usuário específico:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a41c3-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="a41c3-120">Para o usuário entrou no:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a41c3-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a41c3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a41c3-121">Optional query parameters</span></span>
<span data-ttu-id="a41c3-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a41c3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a41c3-123">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a41c3-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="a41c3-124">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a41c3-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="a41c3-125">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="a41c3-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="a41c3-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a41c3-126">Request headers</span></span>
| <span data-ttu-id="a41c3-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a41c3-127">Header</span></span>       | <span data-ttu-id="a41c3-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a41c3-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a41c3-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a41c3-129">Authorization</span></span>  | <span data-ttu-id="a41c3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a41c3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a41c3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a41c3-132">Content-Type</span></span>   | <span data-ttu-id="a41c3-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a41c3-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a41c3-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a41c3-134">Request body</span></span>
<span data-ttu-id="a41c3-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a41c3-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a41c3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a41c3-136">Response</span></span>

<span data-ttu-id="a41c3-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a41c3-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a41c3-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a41c3-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="a41c3-139">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="a41c3-139">Example 1: Standard users request</span></span>

<span data-ttu-id="a41c3-140">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a41c3-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="a41c3-141">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="a41c3-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="a41c3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a41c3-142">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="a41c3-143">Exemplo 2: solicitação de usuário conectado</span><span class="sxs-lookup"><span data-stu-id="a41c3-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="a41c3-144">Você pode obter as informações do usuário para o usuário conectado, substituindo `/users/{id | userPrincipalName}` por `/me`.</span><span class="sxs-lookup"><span data-stu-id="a41c3-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="a41c3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a41c3-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="a41c3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a41c3-146">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="a41c3-147">Exemplo 3: solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="a41c3-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="a41c3-148">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a41c3-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="a41c3-149">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="a41c3-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="a41c3-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a41c3-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="a41c3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a41c3-151">Response</span></span>
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
