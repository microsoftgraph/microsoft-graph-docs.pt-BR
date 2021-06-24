---
title: Obter um usuário
description: Recuperar as propriedades e os relacionamentos do objeto user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b0fecfe948c59fe184e82f71e83d835cee74c7ff
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107694"
---
# <a name="get-a-user"></a><span data-ttu-id="d0523-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="d0523-103">Get a user</span></span>

<span data-ttu-id="d0523-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0523-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0523-105">Recuperar as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="d0523-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="d0523-p101">Observação: obter um usuário retorna uma coleção padrão de propriedades somente (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` para obter outras propriedades e relacionamentos para o objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d0523-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0523-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0523-108">Permissions</span></span>
<span data-ttu-id="d0523-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0523-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0523-111">Permission type</span></span>      | <span data-ttu-id="d0523-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0523-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0523-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0523-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d0523-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0523-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0523-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0523-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0523-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0523-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="d0523-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0523-117">Application</span></span> | <span data-ttu-id="d0523-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0523-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="d0523-119">Chamar o ponto de extremidade `/me` exige um usuário conectado e, portanto, uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="d0523-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="d0523-120">Não há suporte para permissões do aplicativo ao usar o ponto de extremidade `/me`.</span><span class="sxs-lookup"><span data-stu-id="d0523-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0523-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0523-121">HTTP request</span></span>
<span data-ttu-id="d0523-122">Para um usuário específico:</span><span class="sxs-lookup"><span data-stu-id="d0523-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

><span data-ttu-id="d0523-123">**Nota:**</span><span class="sxs-lookup"><span data-stu-id="d0523-123">**Note:**</span></span>
> + <span data-ttu-id="d0523-p104">Quando o **userPrincipalName** começar com um caractere `$`, remova a barra (/) após `/users` e coloque o **userPrincipalName** entre parênteses e aspas simples. Por exemplo, `/users('$AdeleVance@contoso.com')`. Para detalhes, consultar a lista de [problemas conhecidos](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="d0523-p104">When the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For example, `/users('$AdeleVance@contoso.com')`. For details, see the [known issues](/graph/known-issues#users) list.</span></span>
> + <span data-ttu-id="d0523-127">Para consultar um usuário B2B usando o **usuárioPrincipalName**, codifique o caractere hash (#).</span><span class="sxs-lookup"><span data-stu-id="d0523-127">To query a B2B user using the **userPrincipalName**, encode the hash (#) character.</span></span> <span data-ttu-id="d0523-128">Ou seja, substituir o símbolo `#` por `%23`.</span><span class="sxs-lookup"><span data-stu-id="d0523-128">That is, replace the `#` symbol with `%23`.</span></span> <span data-ttu-id="d0523-129">Por exemplo, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="d0523-129">For example, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span></span>

<span data-ttu-id="d0523-130">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="d0523-130">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0523-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0523-131">Optional query parameters</span></span>
<span data-ttu-id="d0523-132">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0523-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="d0523-133">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="d0523-133">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="d0523-134">Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="d0523-134">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="d0523-135">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="d0523-135">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0523-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0523-136">Request headers</span></span>
| <span data-ttu-id="d0523-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0523-137">Header</span></span>       | <span data-ttu-id="d0523-138">Valor</span><span class="sxs-lookup"><span data-stu-id="d0523-138">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d0523-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0523-139">Authorization</span></span>  | <span data-ttu-id="d0523-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0523-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0523-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0523-142">Content-Type</span></span>   | <span data-ttu-id="d0523-143">application/json</span><span class="sxs-lookup"><span data-stu-id="d0523-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0523-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0523-144">Request body</span></span>
<span data-ttu-id="d0523-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0523-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0523-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0523-146">Response</span></span>

<span data-ttu-id="d0523-147">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0523-147">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="d0523-148">Esse método retorna `202 Accepted` quando a solicitação tiver sido processada com sucesso, mas o servidor requer mais tempo para concluir as operações de segundo plano relacionadas.</span><span class="sxs-lookup"><span data-stu-id="d0523-148">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="d0523-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0523-149">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="d0523-150">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="d0523-150">Example 1: Standard users request</span></span>

<span data-ttu-id="d0523-151">Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="d0523-151">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="d0523-152">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0523-152">This example illustrates the default request and response.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_user_1"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="d0523-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0523-153">Response</span></span>

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
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="d0523-154">Exemplo 2: solicitação de usuário conectado</span><span class="sxs-lookup"><span data-stu-id="d0523-154">Example 2: Signed-in user request</span></span>

<span data-ttu-id="d0523-155">Você pode obter as informações do usuário para o usuário conectado, substituindo `/users/{id | userPrincipalName}` por `/me`.</span><span class="sxs-lookup"><span data-stu-id="d0523-155">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="d0523-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0523-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0523-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0523-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="d0523-158">C#</span><span class="sxs-lookup"><span data-stu-id="d0523-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0523-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0523-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0523-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0523-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0523-161">Java</span><span class="sxs-lookup"><span data-stu-id="d0523-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0523-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0523-162">Response</span></span>

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
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="d0523-163">Exemplo 3: solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="d0523-163">Example 3: Users request using $select</span></span>

<span data-ttu-id="d0523-164">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="d0523-164">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="d0523-165">Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="d0523-165">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="d0523-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0523-166">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d0523-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0523-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="d0523-168">C#</span><span class="sxs-lookup"><span data-stu-id="d0523-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0523-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0523-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0523-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0523-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0523-171">Java</span><span class="sxs-lookup"><span data-stu-id="d0523-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0523-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0523-172">Response</span></span>
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
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "postalCode": "98004"
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
