---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 46f4187f184c9303466161d575634224d1961eae
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49030260"
---
# <a name="list-users"></a><span data-ttu-id="aec88-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="aec88-103">List users</span></span>

<span data-ttu-id="aec88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aec88-105">Recupere uma lista de objetos de [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="aec88-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="aec88-p101">Essa operação retorna por padrão apenas um subconjunto das propriedades mais comumente usadas para cada usuário. Essas propriedades _padrão_ são observadas na seção [Propriedades](../resources/user.md#properties). Para obter propriedades que _não_ são retornadas por padrão, execute uma [operação GET](user-get.md) do usuário e especifique as propriedades em uma opção de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="aec88-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="aec88-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="aec88-109">Permissions</span></span>

<span data-ttu-id="aec88-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec88-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aec88-112">Permission type</span></span>      | <span data-ttu-id="aec88-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aec88-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aec88-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aec88-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aec88-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aec88-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aec88-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aec88-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec88-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aec88-117">Not supported.</span></span>    |
|<span data-ttu-id="aec88-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aec88-118">Application</span></span> | <span data-ttu-id="aec88-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec88-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aec88-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aec88-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aec88-121">Optional query parameters</span></span>

<span data-ttu-id="aec88-p103">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count` e `$filter`. Você pode usar `$search` na propriedade **displayName**. Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os parâmetros de consulta `$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando está disponível no índice. Os parâmetros `$count` e `$search` não estão disponíveis atualmente em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="aec88-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aec88-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-127">Request headers</span></span>

| <span data-ttu-id="aec88-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aec88-128">Header</span></span> | <span data-ttu-id="aec88-129">Valor</span><span class="sxs-lookup"><span data-stu-id="aec88-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="aec88-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="aec88-130">Authorization</span></span> | <span data-ttu-id="aec88-131">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="aec88-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="aec88-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="aec88-132">ConsistencyLevel</span></span> | <span data-ttu-id="aec88-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="aec88-133">eventual.</span></span> <span data-ttu-id="aec88-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="aec88-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="aec88-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="aec88-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aec88-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-136">Request body</span></span>

<span data-ttu-id="aec88-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aec88-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aec88-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-138">Response</span></span>

<span data-ttu-id="aec88-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aec88-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aec88-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="aec88-141">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="aec88-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-142">Request</span></span>

<span data-ttu-id="aec88-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aec88-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="aec88-145">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-148">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="aec88-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-149">Response</span></span>

<span data-ttu-id="aec88-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-150">The following is an example of the response.</span></span> 
><span data-ttu-id="aec88-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="aec88-153">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="aec88-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="aec88-154">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="aec88-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="aec88-155">Ao filtrar por **identidades** , você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="aec88-155">When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-156">Request</span></span>

<span data-ttu-id="aec88-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aec88-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="aec88-159">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-162">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="aec88-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-163">Response</span></span>

<span data-ttu-id="aec88-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-164">The following is an example of the response.</span></span> 
> <span data-ttu-id="aec88-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="aec88-167">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="aec88-167">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-168">Request</span></span>

<span data-ttu-id="aec88-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aec88-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="aec88-171">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-174">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="aec88-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-175">Response</span></span>

<span data-ttu-id="aec88-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-176">The following is an example of the response.</span></span> 
> <span data-ttu-id="aec88-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="aec88-179">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="aec88-179">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-180">Request</span></span>

<span data-ttu-id="aec88-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-181">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="aec88-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="aec88-183">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-186">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aec88-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-187">Response</span></span>

<span data-ttu-id="aec88-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-188">The following is an example of the response.</span></span> 
> <span data-ttu-id="aec88-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="aec88-191">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="aec88-191">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-192">Request</span></span>

<span data-ttu-id="aec88-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-193">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="aec88-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="aec88-195">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-198">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aec88-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-199">Response</span></span>

<span data-ttu-id="aec88-200">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-200">The following is an example of the response.</span></span> 
> <span data-ttu-id="aec88-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="aec88-203">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="aec88-203">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-204">Request</span></span>

<span data-ttu-id="aec88-205">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-205">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aec88-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="aec88-207">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-210">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aec88-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-211">Response</span></span>

<span data-ttu-id="aec88-212">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-212">The following is an example of the response.</span></span>

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

<span data-ttu-id="aec88-213">893</span><span class="sxs-lookup"><span data-stu-id="aec88-213">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="aec88-214">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="aec88-214">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-215">Request</span></span>

<span data-ttu-id="aec88-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aec88-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="aec88-218">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-221">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aec88-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-222">Response</span></span>

<span data-ttu-id="aec88-223">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-223">The following is an example of the response.</span></span>
><span data-ttu-id="aec88-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="aec88-226">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="aec88-226">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-227">Request</span></span>

<span data-ttu-id="aec88-228">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aec88-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec88-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="aec88-230">C#</span><span class="sxs-lookup"><span data-stu-id="aec88-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec88-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec88-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec88-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec88-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aec88-233">Java</span><span class="sxs-lookup"><span data-stu-id="aec88-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-wa-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aec88-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-234">Response</span></span>

<span data-ttu-id="aec88-235">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-235">The following is an example of the response.</span></span>
><span data-ttu-id="aec88-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="aec88-238">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="aec88-238">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="aec88-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec88-239">Request</span></span>

<span data-ttu-id="aec88-240">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec88-240">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="aec88-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec88-241">Response</span></span>

<span data-ttu-id="aec88-242">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec88-242">The following is an example of the response.</span></span> 
> <span data-ttu-id="aec88-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec88-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
