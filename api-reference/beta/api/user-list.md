---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bd56e0b6849626bc31a5397ce47fae8a1279aed2
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352393"
---
# <a name="list-users"></a><span data-ttu-id="d480f-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="d480f-103">List users</span></span>

<span data-ttu-id="d480f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d480f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d480f-105">Recupere uma lista de objetos de [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d480f-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="d480f-p101">Essa operação retorna por padrão apenas um subconjunto das propriedades mais comumente usadas para cada usuário. Essas propriedades _padrão_ são observadas na seção [Propriedades](../resources/user.md#properties). Para obter propriedades que _não_ são retornadas por padrão, execute uma [operação GET](user-get.md) do usuário e especifique as propriedades em uma opção de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="d480f-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="d480f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d480f-109">Permissions</span></span>

<span data-ttu-id="d480f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d480f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d480f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d480f-112">Permission type</span></span>      | <span data-ttu-id="d480f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d480f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d480f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d480f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d480f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d480f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d480f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d480f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d480f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d480f-117">Not supported.</span></span>    |
|<span data-ttu-id="d480f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d480f-118">Application</span></span> | <span data-ttu-id="d480f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d480f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d480f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d480f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d480f-121">Optional query parameters</span></span>

<span data-ttu-id="d480f-p103">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count` e `$filter`. Você pode usar `$search` na propriedade **displayName**. Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os parâmetros de consulta `$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando está disponível no índice. Os parâmetros `$count` e `$search` não estão disponíveis atualmente em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="d480f-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d480f-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-127">Request headers</span></span>

| <span data-ttu-id="d480f-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d480f-128">Header</span></span> | <span data-ttu-id="d480f-129">Valor</span><span class="sxs-lookup"><span data-stu-id="d480f-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="d480f-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d480f-130">Authorization</span></span> | <span data-ttu-id="d480f-131">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="d480f-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="d480f-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="d480f-132">ConsistencyLevel</span></span> | <span data-ttu-id="d480f-p104">eventual. Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o parâmetro de consulta `$orderby`. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="d480f-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d480f-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-136">Request body</span></span>

<span data-ttu-id="d480f-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d480f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d480f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-138">Response</span></span>

<span data-ttu-id="d480f-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d480f-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d480f-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="d480f-141">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="d480f-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-142">Request</span></span>

<span data-ttu-id="d480f-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d480f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="d480f-145">C#</span><span class="sxs-lookup"><span data-stu-id="d480f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d480f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d480f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d480f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d480f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d480f-148">Java</span><span class="sxs-lookup"><span data-stu-id="d480f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d480f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-149">Response</span></span>

<span data-ttu-id="d480f-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-150">The following is an example of the response.</span></span> 
><span data-ttu-id="d480f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="d480f-153">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="d480f-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="d480f-154">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="d480f-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="d480f-155">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="d480f-155">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="d480f-156">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="d480f-156">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="d480f-157">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="d480f-157">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-158">Request</span></span>

<span data-ttu-id="d480f-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d480f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="d480f-161">C#</span><span class="sxs-lookup"><span data-stu-id="d480f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d480f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d480f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d480f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d480f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d480f-164">Java</span><span class="sxs-lookup"><span data-stu-id="d480f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d480f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-165">Response</span></span>

<span data-ttu-id="d480f-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="d480f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="d480f-169">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="d480f-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-170">Request</span></span>

<span data-ttu-id="d480f-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d480f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="d480f-173">C#</span><span class="sxs-lookup"><span data-stu-id="d480f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d480f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d480f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d480f-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d480f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d480f-176">Java</span><span class="sxs-lookup"><span data-stu-id="d480f-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d480f-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-177">Response</span></span>

<span data-ttu-id="d480f-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-178">The following is an example of the response.</span></span> 
> <span data-ttu-id="d480f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="d480f-181">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="d480f-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-182">Request</span></span>

<span data-ttu-id="d480f-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d480f-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="d480f-185">C#</span><span class="sxs-lookup"><span data-stu-id="d480f-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d480f-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d480f-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d480f-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d480f-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d480f-188">Java</span><span class="sxs-lookup"><span data-stu-id="d480f-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d480f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-189">Response</span></span>

<span data-ttu-id="d480f-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-190">The following is an example of the response.</span></span> 
> <span data-ttu-id="d480f-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="d480f-193">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="d480f-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-194">Request</span></span>

<span data-ttu-id="d480f-195">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-195">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d480f-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="d480f-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="d480f-197">C#</span><span class="sxs-lookup"><span data-stu-id="d480f-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d480f-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d480f-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d480f-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d480f-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d480f-200">Java</span><span class="sxs-lookup"><span data-stu-id="d480f-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d480f-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-201">Response</span></span>

<span data-ttu-id="d480f-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-202">The following is an example of the response.</span></span> 
> <span data-ttu-id="d480f-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="d480f-205">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="d480f-205">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-206">Request</span></span>

<span data-ttu-id="d480f-207">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-207">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d480f-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-208">Response</span></span>

<span data-ttu-id="d480f-209">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-209">The following is an example of the response.</span></span>

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

<span data-ttu-id="d480f-210">893</span><span class="sxs-lookup"><span data-stu-id="d480f-210">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d480f-211">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d480f-211">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-212">Request</span></span>

<span data-ttu-id="d480f-213">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-213">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d480f-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-214">Response</span></span>

<span data-ttu-id="d480f-215">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-215">The following is an example of the response.</span></span>
><span data-ttu-id="d480f-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="d480f-218">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d480f-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-219">Request</span></span>

<span data-ttu-id="d480f-220">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-220">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d480f-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-221">Response</span></span>

<span data-ttu-id="d480f-222">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-222">The following is an example of the response.</span></span>
><span data-ttu-id="d480f-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="d480f-225">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d480f-225">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d480f-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d480f-226">Request</span></span>

<span data-ttu-id="d480f-227">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d480f-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d480f-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="d480f-228">Response</span></span>

<span data-ttu-id="d480f-229">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d480f-229">The following is an example of the response.</span></span> 
> <span data-ttu-id="d480f-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d480f-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
