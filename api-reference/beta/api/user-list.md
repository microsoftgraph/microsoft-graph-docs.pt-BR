---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f084afca991937b13b96be19c82b6bdcd9da27fb
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081954"
---
# <a name="list-users"></a><span data-ttu-id="bfcbb-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="bfcbb-103">List users</span></span>

<span data-ttu-id="bfcbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfcbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfcbb-105">Recupere uma lista de objetos de [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bfcbb-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="bfcbb-p101">Essa operação retorna por padrão apenas um subconjunto das propriedades mais comumente usadas para cada usuário. Essas propriedades _padrão_ são observadas na seção [Propriedades](../resources/user.md#properties). Para obter propriedades que _não_ são retornadas por padrão, execute uma [operação GET](user-get.md) do usuário e especifique as propriedades em uma opção de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfcbb-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfcbb-109">Permissions</span></span>

<span data-ttu-id="bfcbb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfcbb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfcbb-112">Permission type</span></span>      | <span data-ttu-id="bfcbb-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfcbb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfcbb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfcbb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bfcbb-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfcbb-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bfcbb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfcbb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfcbb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-117">Not supported.</span></span>    |
|<span data-ttu-id="bfcbb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfcbb-118">Application</span></span> | <span data-ttu-id="bfcbb-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfcbb-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfcbb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfcbb-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfcbb-121">Optional query parameters</span></span>

<span data-ttu-id="bfcbb-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="bfcbb-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="bfcbb-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="bfcbb-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="bfcbb-126">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-126">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfcbb-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-127">Request headers</span></span>

| <span data-ttu-id="bfcbb-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bfcbb-128">Header</span></span> | <span data-ttu-id="bfcbb-129">Valor</span><span class="sxs-lookup"><span data-stu-id="bfcbb-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="bfcbb-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfcbb-130">Authorization</span></span> | <span data-ttu-id="bfcbb-131">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="bfcbb-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="bfcbb-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="bfcbb-132">ConsistencyLevel</span></span> | <span data-ttu-id="bfcbb-p104">eventual. Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o parâmetro de consulta `$orderby`. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfcbb-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-136">Request body</span></span>

<span data-ttu-id="bfcbb-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfcbb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-138">Response</span></span>

<span data-ttu-id="bfcbb-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfcbb-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bfcbb-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="bfcbb-141">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="bfcbb-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-142">Request</span></span>

<span data-ttu-id="bfcbb-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfcbb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="bfcbb-145">C#</span><span class="sxs-lookup"><span data-stu-id="bfcbb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfcbb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcbb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfcbb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfcbb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfcbb-148">Java</span><span class="sxs-lookup"><span data-stu-id="bfcbb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bfcbb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-149">Response</span></span>

<span data-ttu-id="bfcbb-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-150">The following is an example of the response.</span></span> 
><span data-ttu-id="bfcbb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="bfcbb-153">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="bfcbb-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="bfcbb-154">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="bfcbb-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="bfcbb-155">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-155">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-156">Request</span></span>

<span data-ttu-id="bfcbb-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfcbb-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="bfcbb-159">C#</span><span class="sxs-lookup"><span data-stu-id="bfcbb-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfcbb-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcbb-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfcbb-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfcbb-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfcbb-162">Java</span><span class="sxs-lookup"><span data-stu-id="bfcbb-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bfcbb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-163">Response</span></span>

<span data-ttu-id="bfcbb-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-164">The following is an example of the response.</span></span> 
> <span data-ttu-id="bfcbb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="bfcbb-167">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="bfcbb-167">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-168">Request</span></span>

<span data-ttu-id="bfcbb-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bfcbb-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="bfcbb-171">C#</span><span class="sxs-lookup"><span data-stu-id="bfcbb-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfcbb-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcbb-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfcbb-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfcbb-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfcbb-174">Java</span><span class="sxs-lookup"><span data-stu-id="bfcbb-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bfcbb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-175">Response</span></span>

<span data-ttu-id="bfcbb-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-176">The following is an example of the response.</span></span> 
> <span data-ttu-id="bfcbb-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="bfcbb-179">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="bfcbb-179">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-180">Request</span></span>

<span data-ttu-id="bfcbb-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfcbb-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="bfcbb-183">C#</span><span class="sxs-lookup"><span data-stu-id="bfcbb-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfcbb-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcbb-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfcbb-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfcbb-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfcbb-186">Java</span><span class="sxs-lookup"><span data-stu-id="bfcbb-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bfcbb-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-187">Response</span></span>

<span data-ttu-id="bfcbb-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-188">The following is an example of the response.</span></span> 
> <span data-ttu-id="bfcbb-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="bfcbb-191">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="bfcbb-191">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-192">Request</span></span>

<span data-ttu-id="bfcbb-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-193">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfcbb-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcbb-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="bfcbb-195">C#</span><span class="sxs-lookup"><span data-stu-id="bfcbb-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfcbb-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcbb-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfcbb-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfcbb-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfcbb-198">Java</span><span class="sxs-lookup"><span data-stu-id="bfcbb-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bfcbb-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-199">Response</span></span>

<span data-ttu-id="bfcbb-200">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-200">The following is an example of the response.</span></span> 
> <span data-ttu-id="bfcbb-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="bfcbb-203">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="bfcbb-203">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-204">Request</span></span>

<span data-ttu-id="bfcbb-205">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-205">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bfcbb-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-206">Response</span></span>

<span data-ttu-id="bfcbb-207">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-207">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="bfcbb-208">893</span><span class="sxs-lookup"><span data-stu-id="bfcbb-208">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="bfcbb-209">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="bfcbb-209">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-210">Request</span></span>

<span data-ttu-id="bfcbb-211">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-211">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bfcbb-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-212">Response</span></span>

<span data-ttu-id="bfcbb-213">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-213">The following is an example of the response.</span></span>
><span data-ttu-id="bfcbb-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="bfcbb-216">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="bfcbb-216">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-217">Request</span></span>

<span data-ttu-id="bfcbb-218">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-218">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bfcbb-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-219">Response</span></span>

<span data-ttu-id="bfcbb-220">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-220">The following is an example of the response.</span></span>
><span data-ttu-id="bfcbb-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="bfcbb-223">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="bfcbb-223">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="bfcbb-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfcbb-224">Request</span></span>

<span data-ttu-id="bfcbb-225">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-225">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="bfcbb-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfcbb-226">Response</span></span>

<span data-ttu-id="bfcbb-227">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-227">The following is an example of the response.</span></span> 
> <span data-ttu-id="bfcbb-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfcbb-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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
