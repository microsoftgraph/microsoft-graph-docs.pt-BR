---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cfb2043ed4fc9f885eaad407f62595203af45ce5
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703528"
---
# <a name="list-users"></a><span data-ttu-id="55b8d-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="55b8d-103">List users</span></span>

<span data-ttu-id="55b8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55b8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55b8d-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="55b8d-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="55b8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55b8d-106">Permissions</span></span>

<span data-ttu-id="55b8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55b8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55b8d-109">Permission type</span></span>      | <span data-ttu-id="55b8d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55b8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55b8d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55b8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55b8d-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55b8d-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55b8d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55b8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55b8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55b8d-114">Not supported.</span></span>    |
|<span data-ttu-id="55b8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55b8d-115">Application</span></span> | <span data-ttu-id="55b8d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b8d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55b8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55b8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55b8d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55b8d-118">Optional query parameters</span></span>

<span data-ttu-id="55b8d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="55b8d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="55b8d-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="55b8d-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="55b8d-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="55b8d-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="55b8d-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="55b8d-123">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="55b8d-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="55b8d-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="55b8d-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> <span data-ttu-id="55b8d-125">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="55b8d-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="55b8d-126">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="55b8d-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="55b8d-p104">Certas propriedades não podem ser retornadas em uma coleção de usuário. As seguintes propriedades terão suporte apenas [ao recuperar um único usuário:](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="55b8d-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="55b8d-129">As propriedades a seguir não têm suporte em contas pessoais da Microsoft e serão `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span><span class="sxs-lookup"><span data-stu-id="55b8d-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55b8d-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-130">Request headers</span></span>

| <span data-ttu-id="55b8d-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55b8d-131">Header</span></span>        | <span data-ttu-id="55b8d-132">Valor</span><span class="sxs-lookup"><span data-stu-id="55b8d-132">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="55b8d-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="55b8d-133">Authorization</span></span> | <span data-ttu-id="55b8d-134">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="55b8d-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="55b8d-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="55b8d-135">ConsistencyLevel</span></span> | <span data-ttu-id="55b8d-136">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="55b8d-136">eventual.</span></span> <span data-ttu-id="55b8d-137">Este cabeçalho e `$count` são necessários ao usar `$search`, ou ao usar o `$filter` com o parâmetro de consulta `$orderby` ou `$filter` com o operador lógico `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="55b8d-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="55b8d-138">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="55b8d-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55b8d-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-139">Request body</span></span>

<span data-ttu-id="55b8d-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55b8d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55b8d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-141">Response</span></span>

<span data-ttu-id="55b8d-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="55b8d-143">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="55b8d-143">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="55b8d-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55b8d-144">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="55b8d-145">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="55b8d-145">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-146">Request</span></span>

<span data-ttu-id="55b8d-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55b8d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="55b8d-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="55b8d-149">C#</span><span class="sxs-lookup"><span data-stu-id="55b8d-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55b8d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55b8d-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55b8d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55b8d-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55b8d-152">Java</span><span class="sxs-lookup"><span data-stu-id="55b8d-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55b8d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-153">Response</span></span>

<span data-ttu-id="55b8d-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-154">The following is an example of the response.</span></span>

><span data-ttu-id="55b8d-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="55b8d-156">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="55b8d-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-157">Request</span></span>

<span data-ttu-id="55b8d-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-158">The following is an example of the request.</span></span>

><span data-ttu-id="55b8d-159">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="55b8d-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="55b8d-160">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="55b8d-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="55b8d-161">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="55b8d-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="55b8d-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="55b8d-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="55b8d-163">C#</span><span class="sxs-lookup"><span data-stu-id="55b8d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55b8d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55b8d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55b8d-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55b8d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55b8d-166">Java</span><span class="sxs-lookup"><span data-stu-id="55b8d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55b8d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-167">Response</span></span>

<span data-ttu-id="55b8d-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="55b8d-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="55b8d-170">Exemplo 3: obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="55b8d-170">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-171">Request</span></span>

<span data-ttu-id="55b8d-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55b8d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-173">Response</span></span>

<span data-ttu-id="55b8d-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="55b8d-175">Exemplo 4: utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="55b8d-175">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-176">Request</span></span>

<span data-ttu-id="55b8d-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55b8d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-178">Response</span></span>

<span data-ttu-id="55b8d-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-179">The following is an example of the response.</span></span>

><span data-ttu-id="55b8d-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="55b8d-181">Exemplo 5: utilize $filtro para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="55b8d-181">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-182">Request</span></span>

<span data-ttu-id="55b8d-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55b8d-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="55b8d-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="55b8d-185">C#</span><span class="sxs-lookup"><span data-stu-id="55b8d-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55b8d-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55b8d-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55b8d-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55b8d-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55b8d-188">Java</span><span class="sxs-lookup"><span data-stu-id="55b8d-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55b8d-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-189">Response</span></span>

<span data-ttu-id="55b8d-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-190">The following is an example of the response.</span></span>

><span data-ttu-id="55b8d-191">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-191">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="55b8d-192">Exemplo 6: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="55b8d-192">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-193">Request</span></span>

<span data-ttu-id="55b8d-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55b8d-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-195">Response</span></span>

<span data-ttu-id="55b8d-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-196">The following is an example of the response.</span></span>

><span data-ttu-id="55b8d-197">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-197">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="55b8d-198">Exemplo 7: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras “wa”, ou as letras “para” incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="55b8d-198">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-199">Request</span></span>

<span data-ttu-id="55b8d-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55b8d-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-201">Response</span></span>

<span data-ttu-id="55b8d-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-202">The following is an example of the response.</span></span>

> <span data-ttu-id="55b8d-203">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55b8d-203">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="55b8d-204">Exemplo 8: Use $ filter para obter usuários que receberam uma licença específica</span><span class="sxs-lookup"><span data-stu-id="55b8d-204">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="55b8d-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55b8d-205">Request</span></span>

<span data-ttu-id="55b8d-206">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55b8d-206">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="55b8d-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="55b8d-207">Response</span></span>

<span data-ttu-id="55b8d-208">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55b8d-208">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,mail,assignedLicenses)",
  "value": [
    {
      "id": "cb4954e8-467f-4a6d-a8c8-28b9034fadbc",
      "mail": "admin@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    },
    {
      "id": "81a133c2-bdf2-4e67-8755-7264366b04ee",
      "mail": "DebraB@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
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
