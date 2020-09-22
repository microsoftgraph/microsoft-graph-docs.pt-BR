---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6557f9656a1de807266afa8381c47250f2c9d52b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069600"
---
# <a name="get-a-user"></a><span data-ttu-id="b9385-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="b9385-103">Get a user</span></span>

<span data-ttu-id="b9385-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9385-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9385-105">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="b9385-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="b9385-p101">Observação: obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b9385-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9385-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9385-108">Permissions</span></span>
<span data-ttu-id="b9385-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9385-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9385-111">Permission type</span></span>      | <span data-ttu-id="b9385-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9385-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9385-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9385-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9385-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9385-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9385-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9385-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9385-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9385-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="b9385-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9385-117">Application</span></span> | <span data-ttu-id="b9385-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9385-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="b9385-119">Chamar o ponto de extremidade `/me` exige um usuário conectado e, portanto, uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="b9385-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="b9385-120">Não há suporte para permissões do aplicativo ao usar o ponto de extremidade `/me`.</span><span class="sxs-lookup"><span data-stu-id="b9385-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="b9385-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9385-121">HTTP request</span></span>
<span data-ttu-id="b9385-122">Para um usuário específico:</span><span class="sxs-lookup"><span data-stu-id="b9385-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="b9385-123">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="b9385-123">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9385-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9385-124">Optional query parameters</span></span>
<span data-ttu-id="b9385-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9385-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b9385-126">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="b9385-126">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="b9385-127">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="b9385-127">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="b9385-128">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="b9385-128">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9385-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9385-129">Request headers</span></span>
| <span data-ttu-id="b9385-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9385-130">Header</span></span>       | <span data-ttu-id="b9385-131">Valor</span><span class="sxs-lookup"><span data-stu-id="b9385-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b9385-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9385-132">Authorization</span></span>  | <span data-ttu-id="b9385-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9385-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9385-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9385-135">Content-Type</span></span>   | <span data-ttu-id="b9385-136">application/json</span><span class="sxs-lookup"><span data-stu-id="b9385-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9385-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9385-137">Request body</span></span>
<span data-ttu-id="b9385-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9385-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9385-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9385-139">Response</span></span>

<span data-ttu-id="b9385-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9385-140">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="b9385-141">Esse método retorna `202 Accepted` quando a solicitação tiver sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="b9385-141">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="b9385-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9385-142">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="b9385-143">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="b9385-143">Example 1: Standard users request</span></span>

<span data-ttu-id="b9385-144">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="b9385-144">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="b9385-145">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9385-145">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="b9385-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9385-146">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="b9385-147">Exemplo 2: solicitação de usuário conectado</span><span class="sxs-lookup"><span data-stu-id="b9385-147">Example 2: Signed-in user request</span></span>

<span data-ttu-id="b9385-148">Você pode obter as informações do usuário para o usuário conectado, substituindo `/users/{id | userPrincipalName}` por `/me`.</span><span class="sxs-lookup"><span data-stu-id="b9385-148">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="b9385-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9385-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9385-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9385-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="b9385-151">C#</span><span class="sxs-lookup"><span data-stu-id="b9385-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9385-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9385-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9385-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9385-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9385-154">Java</span><span class="sxs-lookup"><span data-stu-id="b9385-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9385-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9385-155">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="b9385-156">Exemplo 3: solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="b9385-156">Example 3: Users request using $select</span></span>

<span data-ttu-id="b9385-157">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="b9385-157">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="b9385-158">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="b9385-158">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="b9385-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9385-159">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="b9385-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9385-160">Response</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

