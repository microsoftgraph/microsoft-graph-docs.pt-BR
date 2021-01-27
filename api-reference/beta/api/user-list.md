---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0439f9ac1e0e1de4772dd300ff064d63c607016a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013409"
---
# <a name="list-users"></a><span data-ttu-id="3ef4b-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="3ef4b-103">List users</span></span>

<span data-ttu-id="3ef4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ef4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef4b-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3ef4b-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="3ef4b-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="3ef4b-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="3ef4b-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="3ef4b-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](user-get.md) para o usuário e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef4b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ef4b-109">Permissions</span></span>

<span data-ttu-id="3ef4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ef4b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ef4b-112">Permission type</span></span>      | <span data-ttu-id="3ef4b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ef4b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ef4b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ef4b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3ef4b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ef4b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3ef4b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ef4b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ef4b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-117">Not supported.</span></span>    |
|<span data-ttu-id="3ef4b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ef4b-118">Application</span></span> | <span data-ttu-id="3ef4b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ef4b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ef4b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ef4b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ef4b-121">Optional query parameters</span></span>

<span data-ttu-id="3ef4b-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="3ef4b-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="3ef4b-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3ef4b-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="3ef4b-126">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-126">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ef4b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-127">Request headers</span></span>

| <span data-ttu-id="3ef4b-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ef4b-128">Header</span></span> | <span data-ttu-id="3ef4b-129">Valor</span><span class="sxs-lookup"><span data-stu-id="3ef4b-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="3ef4b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ef4b-130">Authorization</span></span> | <span data-ttu-id="3ef4b-131">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="3ef4b-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="3ef4b-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3ef4b-132">ConsistencyLevel</span></span> | <span data-ttu-id="3ef4b-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-133">eventual.</span></span> <span data-ttu-id="3ef4b-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="3ef4b-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ef4b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-136">Request body</span></span>

<span data-ttu-id="3ef4b-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ef4b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-138">Response</span></span>

<span data-ttu-id="3ef4b-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ef4b-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ef4b-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="3ef4b-141">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="3ef4b-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-142">Request</span></span>

<span data-ttu-id="3ef4b-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef4b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="3ef4b-145">C#</span><span class="sxs-lookup"><span data-stu-id="3ef4b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef4b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef4b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef4b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef4b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef4b-148">Java</span><span class="sxs-lookup"><span data-stu-id="3ef4b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3ef4b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-149">Response</span></span>

<span data-ttu-id="3ef4b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-150">The following is an example of the response.</span></span> 
><span data-ttu-id="3ef4b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="3ef4b-153">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="3ef4b-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="3ef4b-154">Encontrar uma conta de usuário usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="3ef4b-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="3ef4b-155">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-155">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="3ef4b-156">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="3ef4b-156">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="3ef4b-157">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-157">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-158">Request</span></span>

<span data-ttu-id="3ef4b-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef4b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="3ef4b-161">C#</span><span class="sxs-lookup"><span data-stu-id="3ef4b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef4b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef4b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef4b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef4b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef4b-164">Java</span><span class="sxs-lookup"><span data-stu-id="3ef4b-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3ef4b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-165">Response</span></span>

<span data-ttu-id="3ef4b-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="3ef4b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="3ef4b-169">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="3ef4b-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-170">Request</span></span>

<span data-ttu-id="3ef4b-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef4b-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="3ef4b-173">C#</span><span class="sxs-lookup"><span data-stu-id="3ef4b-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef4b-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef4b-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef4b-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef4b-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef4b-176">Java</span><span class="sxs-lookup"><span data-stu-id="3ef4b-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3ef4b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-177">Response</span></span>

<span data-ttu-id="3ef4b-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-178">The following is an example of the response.</span></span> 
> <span data-ttu-id="3ef4b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="3ef4b-181">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="3ef4b-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-182">Request</span></span>

<span data-ttu-id="3ef4b-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef4b-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="3ef4b-185">C#</span><span class="sxs-lookup"><span data-stu-id="3ef4b-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef4b-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef4b-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef4b-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef4b-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef4b-188">Java</span><span class="sxs-lookup"><span data-stu-id="3ef4b-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ef4b-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-189">Response</span></span>

<span data-ttu-id="3ef4b-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-190">The following is an example of the response.</span></span> 
> <span data-ttu-id="3ef4b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="3ef4b-193">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="3ef4b-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-194">Request</span></span>

<span data-ttu-id="3ef4b-195">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-195">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="3ef4b-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-196">Response</span></span>

<span data-ttu-id="3ef4b-197">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-197">The following is an example of the response.</span></span> 
> <span data-ttu-id="3ef4b-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="3ef4b-200">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="3ef4b-200">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-201">Request</span></span>

<span data-ttu-id="3ef4b-202">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-202">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3ef4b-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-203">Response</span></span>

<span data-ttu-id="3ef4b-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-204">The following is an example of the response.</span></span>

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

<span data-ttu-id="3ef4b-205">893</span><span class="sxs-lookup"><span data-stu-id="3ef4b-205">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3ef4b-206">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3ef4b-206">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-207">Request</span></span>

<span data-ttu-id="3ef4b-208">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-208">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3ef4b-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-209">Response</span></span>

<span data-ttu-id="3ef4b-210">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-210">The following is an example of the response.</span></span>
><span data-ttu-id="3ef4b-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="3ef4b-213">Exemplo 8: utilize $filter para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3ef4b-213">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-214">Request</span></span>

<span data-ttu-id="3ef4b-215">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-215">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef4b-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef4b-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3ef4b-217">C#</span><span class="sxs-lookup"><span data-stu-id="3ef4b-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef4b-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef4b-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef4b-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef4b-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef4b-220">Java</span><span class="sxs-lookup"><span data-stu-id="3ef4b-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ef4b-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-221">Response</span></span>

<span data-ttu-id="3ef4b-222">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-222">The following is an example of the response.</span></span>

><span data-ttu-id="3ef4b-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count": 1,
  "value": [
    {
      "displayName": "Grady Archie",
      "givenName": "Grady",
      "jobTitle": "Designer",
      "mail": "GradyA@contoso.com",
      "userPrincipalName": "GradyA@contoso.com",
      "id": "e8b753b5-4117-464e-9a08-713e1ff266b3"
      }
    ]
}
```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="3ef4b-225">Exemplo 9: utilize $search para obter usuários com nomes de exibição que contenham as letras “wa”, incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3ef4b-225">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-226">Request</span></span>

<span data-ttu-id="3ef4b-227">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3ef4b-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-228">Response</span></span>

<span data-ttu-id="3ef4b-229">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-229">The following is an example of the response.</span></span>
><span data-ttu-id="3ef4b-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="3ef4b-232">Exemplo 10: utilize $search para obter grupos com nomes de exibição que contenham as letras “wa”, ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3ef4b-232">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3ef4b-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef4b-233">Request</span></span>

<span data-ttu-id="3ef4b-234">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-234">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3ef4b-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef4b-235">Response</span></span>

<span data-ttu-id="3ef4b-236">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-236">The following is an example of the response.</span></span> 
> <span data-ttu-id="3ef4b-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef4b-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
