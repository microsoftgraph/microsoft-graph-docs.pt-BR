---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d4783b0b7788da04e0662dff07782e99505c626e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892688"
---
# <a name="list-users"></a><span data-ttu-id="c703b-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c703b-103">List users</span></span>

<span data-ttu-id="c703b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c703b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c703b-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c703b-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="c703b-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="c703b-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="c703b-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="c703b-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="c703b-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="c703b-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="c703b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c703b-109">Permissions</span></span>

<span data-ttu-id="c703b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c703b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c703b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c703b-112">Permission type</span></span>      | <span data-ttu-id="c703b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c703b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c703b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c703b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c703b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="c703b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span></span> |
|<span data-ttu-id="c703b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c703b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c703b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c703b-117">Not supported.</span></span>    |
|<span data-ttu-id="c703b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c703b-118">Application</span></span> | <span data-ttu-id="c703b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="c703b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c703b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c703b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c703b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c703b-121">Optional query parameters</span></span>

<span data-ttu-id="c703b-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c703b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-123">Request headers</span></span>
| <span data-ttu-id="c703b-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c703b-124">Header</span></span>        | <span data-ttu-id="c703b-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c703b-125">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="c703b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c703b-126">Authorization</span></span> | <span data-ttu-id="c703b-127">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="c703b-127">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c703b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-128">Request body</span></span>

<span data-ttu-id="c703b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c703b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c703b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-130">Response</span></span>

<span data-ttu-id="c703b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c703b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c703b-132">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="c703b-133">Exemplo 1: listar todos os usuários</span><span class="sxs-lookup"><span data-stu-id="c703b-133">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="c703b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-134">Request</span></span>

<span data-ttu-id="c703b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c703b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c703b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c703b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="c703b-137">C#</span><span class="sxs-lookup"><span data-stu-id="c703b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c703b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c703b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c703b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c703b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c703b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-140">Response</span></span>

<span data-ttu-id="c703b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-141">The following is an example of the response.</span></span> 
><span data-ttu-id="c703b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c703b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="c703b-144">Exemplo 2: localizar uma conta de usuário usando o nome de entrada</span><span class="sxs-lookup"><span data-stu-id="c703b-144">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="c703b-145">Encontrar uma conta de usuário em um locatário B2C usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="c703b-145">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="c703b-146">Essa solicitação pode ser usada por um suporte técnico para encontrar uma conta de usuário do cliente, em um locatário B2C (neste exemplo, o locatário B2C é contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="c703b-146">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="c703b-147">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="c703b-147">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="c703b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-148">Request</span></span>

<span data-ttu-id="c703b-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c703b-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c703b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c703b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="c703b-151">C#</span><span class="sxs-lookup"><span data-stu-id="c703b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c703b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c703b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c703b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c703b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c703b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-154">Response</span></span>

<span data-ttu-id="c703b-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-155">The following is an example of the response.</span></span> 
> <span data-ttu-id="c703b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c703b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
    }
  ]
}
```

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="c703b-158">Exemplo 3: listar usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="c703b-158">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="c703b-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-159">Request</span></span>

<span data-ttu-id="c703b-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c703b-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c703b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="c703b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="c703b-162">C#</span><span class="sxs-lookup"><span data-stu-id="c703b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c703b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c703b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c703b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c703b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c703b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-165">Response</span></span>

<span data-ttu-id="c703b-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="c703b-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c703b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="c703b-169">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="c703b-169">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="c703b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-170">Request</span></span>

<span data-ttu-id="c703b-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c703b-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="c703b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-172">Response</span></span>

<span data-ttu-id="c703b-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-173">The following is an example of the response.</span></span> 
> <span data-ttu-id="c703b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c703b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="c703b-176">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="c703b-176">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="c703b-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c703b-177">Request</span></span>

<span data-ttu-id="c703b-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c703b-178">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="c703b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="c703b-179">Response</span></span>

<span data-ttu-id="c703b-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c703b-180">The following is an example of the response.</span></span> 
> <span data-ttu-id="c703b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c703b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
