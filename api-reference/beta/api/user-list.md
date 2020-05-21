---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 50d53f66629e31d490717cd2fcea047d5a5e10ff
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335782"
---
# <a name="list-users"></a><span data-ttu-id="9e89d-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="9e89d-103">List users</span></span>

<span data-ttu-id="9e89d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e89d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e89d-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="9e89d-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="9e89d-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="9e89d-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="9e89d-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="9e89d-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="9e89d-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="9e89d-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e89d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e89d-109">Permissions</span></span>

<span data-ttu-id="9e89d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e89d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e89d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e89d-112">Permission type</span></span>      | <span data-ttu-id="9e89d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e89d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e89d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e89d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e89d-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e89d-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span></span> |
|<span data-ttu-id="9e89d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e89d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e89d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e89d-117">Not supported.</span></span>    |
|<span data-ttu-id="9e89d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e89d-118">Application</span></span> | <span data-ttu-id="9e89d-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e89d-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e89d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e89d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e89d-121">Optional query parameters</span></span>

<span data-ttu-id="9e89d-122">Este método oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="9e89d-122">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9e89d-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="9e89d-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9e89d-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="9e89d-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9e89d-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="9e89d-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e89d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-126">Request headers</span></span>

| <span data-ttu-id="9e89d-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e89d-127">Header</span></span> | <span data-ttu-id="9e89d-128">Valor</span><span class="sxs-lookup"><span data-stu-id="9e89d-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="9e89d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e89d-129">Authorization</span></span> | <span data-ttu-id="9e89d-130">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="9e89d-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="9e89d-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9e89d-131">ConsistencyLevel</span></span> | <span data-ttu-id="9e89d-132">ocorra.</span><span class="sxs-lookup"><span data-stu-id="9e89d-132">eventual.</span></span> <span data-ttu-id="9e89d-133">Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="9e89d-134">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="9e89d-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e89d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-135">Request body</span></span>

<span data-ttu-id="9e89d-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e89d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e89d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-137">Response</span></span>

<span data-ttu-id="9e89d-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e89d-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e89d-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="9e89d-140">Exemplo 1: obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="9e89d-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-141">Request</span></span>

<span data-ttu-id="9e89d-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e89d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="9e89d-144">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9e89d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-147">Response</span></span>

<span data-ttu-id="9e89d-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-148">The following is an example of the response.</span></span> 
><span data-ttu-id="9e89d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="9e89d-151">Exemplo 2: obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="9e89d-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="9e89d-152">Encontre uma conta de usuário usando um nome de logon (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="9e89d-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="9e89d-153">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="9e89d-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-154">Request</span></span>

<span data-ttu-id="9e89d-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e89d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="9e89d-157">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9e89d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-160">Response</span></span>

<span data-ttu-id="9e89d-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="9e89d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="9e89d-164">Exemplo 3: obter usuários, incluindo a última hora de entrada</span><span class="sxs-lookup"><span data-stu-id="9e89d-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-165">Request</span></span>

<span data-ttu-id="9e89d-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e89d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9e89d-168">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9e89d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-171">Response</span></span>

<span data-ttu-id="9e89d-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="9e89d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="9e89d-175">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="9e89d-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-176">Request</span></span>

<span data-ttu-id="9e89d-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-177">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="9e89d-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9e89d-179">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e89d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-182">Response</span></span>

<span data-ttu-id="9e89d-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-183">The following is an example of the response.</span></span> 
> <span data-ttu-id="9e89d-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="9e89d-186">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="9e89d-186">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-187">Request</span></span>

<span data-ttu-id="9e89d-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="9e89d-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="9e89d-190">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e89d-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-193">Response</span></span>

<span data-ttu-id="9e89d-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-194">The following is an example of the response.</span></span> 
> <span data-ttu-id="9e89d-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="9e89d-197">Exemplo 6: obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="9e89d-197">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-198">Request</span></span>

<span data-ttu-id="9e89d-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e89d-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9e89d-201">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e89d-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-204">Response</span></span>

<span data-ttu-id="9e89d-205">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-205">The following is an example of the response.</span></span>

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

<span data-ttu-id="9e89d-206">893</span><span class="sxs-lookup"><span data-stu-id="9e89d-206">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9e89d-207">Exemplo 7: use $filter e $top para obter um usuário com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="9e89d-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-208">Request</span></span>

<span data-ttu-id="9e89d-209">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-209">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e89d-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9e89d-211">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e89d-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-214">Response</span></span>

<span data-ttu-id="9e89d-215">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-215">The following is an example of the response.</span></span>
><span data-ttu-id="9e89d-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="9e89d-218">Exemplo 8: Use $search para obter os usuários com nomes de exibição que contenham as letras "WA", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="9e89d-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-219">Request</span></span>

<span data-ttu-id="9e89d-220">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e89d-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e89d-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9e89d-222">C#</span><span class="sxs-lookup"><span data-stu-id="9e89d-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e89d-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e89d-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e89d-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e89d-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9e89d-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-225">Response</span></span>

<span data-ttu-id="9e89d-226">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-226">The following is an example of the response.</span></span>
><span data-ttu-id="9e89d-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="9e89d-229">Exemplo 9: Use $search para obter os usuários com nomes de exibição que contenham as letras "WA" ou as letras "como", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="9e89d-229">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9e89d-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e89d-230">Request</span></span>

<span data-ttu-id="9e89d-231">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e89d-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9e89d-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e89d-232">Response</span></span>

<span data-ttu-id="9e89d-233">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e89d-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="9e89d-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e89d-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
