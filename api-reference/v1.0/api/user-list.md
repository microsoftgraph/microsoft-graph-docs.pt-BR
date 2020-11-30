---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e32a04a6d10c87dc749b756990b8db1fd1cc3955
ms.sourcegitcommit: 6714f71e0d229f1ab56150a9976b5106b4c8b785
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2020
ms.locfileid: "49368219"
---
# <a name="list-users"></a><span data-ttu-id="d9aa3-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="d9aa3-103">List users</span></span>

<span data-ttu-id="d9aa3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9aa3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9aa3-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d9aa3-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9aa3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9aa3-106">Permissions</span></span>

<span data-ttu-id="d9aa3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9aa3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9aa3-109">Permission type</span></span>      | <span data-ttu-id="d9aa3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9aa3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9aa3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9aa3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9aa3-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9aa3-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9aa3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9aa3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9aa3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-114">Not supported.</span></span>    |
|<span data-ttu-id="d9aa3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9aa3-115">Application</span></span> | <span data-ttu-id="d9aa3-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9aa3-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9aa3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9aa3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9aa3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9aa3-118">Optional query parameters</span></span>

<span data-ttu-id="d9aa3-p102">Este método suporta o [OData query parameters](/graph/query-parameters)para ajudar a personalizar a resposta, incluindo`$search`, `$count`, `$filter`e `$select`. É possível usar a propriedade `$search` no **displayName**. Quando os itens forem adicionados e atualizados por esse recurso, eles serão especialmente indexados para o uso com os parâmetros de consulta`$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando ele está disponível no índice. Os parâmetros `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p102">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="d9aa3-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="d9aa3-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="d9aa3-p103">Para retornar um conjunto de propriedades alternativo, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`. Por exemplo, para retornar o **displayName**, **givenName**, e **postalCode**, adicione o seguinte à sua consulta. `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p103">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter. For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="d9aa3-p104">Certas propriedades não podem ser retornadas em uma coleção de usuário. As seguintes propriedades são suportadas apenas [ao recuperar um único usuário:](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9aa3-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-129">Request headers</span></span>

| <span data-ttu-id="d9aa3-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9aa3-130">Header</span></span>        | <span data-ttu-id="d9aa3-131">Valor</span><span class="sxs-lookup"><span data-stu-id="d9aa3-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="d9aa3-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9aa3-132">Authorization</span></span> | <span data-ttu-id="d9aa3-133">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="d9aa3-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="d9aa3-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="d9aa3-134">ConsistencyLevel</span></span> | <span data-ttu-id="d9aa3-p105">eventual. Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o parâmetro de consulta `$orderby`. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p105">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9aa3-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-138">Request body</span></span>

<span data-ttu-id="d9aa3-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9aa3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-140">Response</span></span>

<span data-ttu-id="d9aa3-p106">Se tiver êxito, este método retorna um código de resposta`200 OK` e a coleção de objetos de[usuário](../resources/user.md) no corpo da resposta. Se uma grande coleção de usuários for retornada, você pode usar uma [paginação em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p106">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body. If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="d9aa3-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9aa3-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="d9aa3-144">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="d9aa3-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-145">Request</span></span>

<span data-ttu-id="d9aa3-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9aa3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9aa3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="d9aa3-148">C#</span><span class="sxs-lookup"><span data-stu-id="d9aa3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9aa3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9aa3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9aa3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9aa3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9aa3-151">Java</span><span class="sxs-lookup"><span data-stu-id="d9aa3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9aa3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-152">Response</span></span>

<span data-ttu-id="d9aa3-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-153">The following is an example of the response.</span></span>

><span data-ttu-id="d9aa3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="d9aa3-156">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="d9aa3-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-157">Request</span></span>

<span data-ttu-id="d9aa3-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-158">The following is an example of the request.</span></span>

><span data-ttu-id="d9aa3-p108">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**. The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN). If a UPN is used, the response will be an empty list.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p108">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**. The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN). If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9aa3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9aa3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="d9aa3-163">C#</span><span class="sxs-lookup"><span data-stu-id="d9aa3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9aa3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9aa3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9aa3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9aa3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9aa3-166">Java</span><span class="sxs-lookup"><span data-stu-id="d9aa3-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9aa3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-167">Response</span></span>

<span data-ttu-id="d9aa3-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="d9aa3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="d9aa3-171">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="d9aa3-171">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-172">Request</span></span>

<span data-ttu-id="d9aa3-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9aa3-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9aa3-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="d9aa3-175">C#</span><span class="sxs-lookup"><span data-stu-id="d9aa3-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9aa3-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9aa3-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9aa3-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9aa3-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9aa3-178">Java</span><span class="sxs-lookup"><span data-stu-id="d9aa3-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9aa3-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-179">Response</span></span>

<span data-ttu-id="d9aa3-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-180">The following is an example of the response.</span></span>

><span data-ttu-id="d9aa3-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="d9aa3-183">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="d9aa3-183">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-184">Request</span></span>

<span data-ttu-id="d9aa3-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9aa3-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9aa3-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="d9aa3-187">C#</span><span class="sxs-lookup"><span data-stu-id="d9aa3-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9aa3-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9aa3-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9aa3-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9aa3-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9aa3-190">Java</span><span class="sxs-lookup"><span data-stu-id="d9aa3-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9aa3-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-191">Response</span></span>

<span data-ttu-id="d9aa3-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-192">The following is an example of the response.</span></span> 

> <span data-ttu-id="d9aa3-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="d9aa3-195">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="d9aa3-195">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-196">Request</span></span>

<span data-ttu-id="d9aa3-197">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
} -->
```http
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="d9aa3-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-198">Response</span></span>

<span data-ttu-id="d9aa3-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-199">The following is an example of the response.</span></span> 

> <span data-ttu-id="d9aa3-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="d9aa3-202">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="d9aa3-202">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-203">Request</span></span>

<span data-ttu-id="d9aa3-204">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-204">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d9aa3-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-205">Response</span></span>

<span data-ttu-id="d9aa3-206">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-206">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d9aa3-207">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d9aa3-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-208">Request</span></span>

<span data-ttu-id="d9aa3-209">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-209">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d9aa3-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-210">Response</span></span>

<span data-ttu-id="d9aa3-211">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-211">The following is an example of the response.</span></span>

><span data-ttu-id="d9aa3-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="d9aa3-214">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d9aa3-214">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-215">Request</span></span>

<span data-ttu-id="d9aa3-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d9aa3-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-217">Response</span></span>

<span data-ttu-id="d9aa3-218">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-218">The following is an example of the response.</span></span>

><span data-ttu-id="d9aa3-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}
```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="d9aa3-221">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d9aa3-221">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d9aa3-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9aa3-222">Request</span></span>

<span data-ttu-id="d9aa3-223">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-223">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d9aa3-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9aa3-224">Response</span></span>

<span data-ttu-id="d9aa3-225">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-225">The following is an example of the response.</span></span>

> <span data-ttu-id="d9aa3-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9aa3-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
