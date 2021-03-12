---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6eec321a319deedc704dc2a2ed508627a2de11ba
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721926"
---
# <a name="list-users"></a><span data-ttu-id="0fa26-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="0fa26-103">List users</span></span>

<span data-ttu-id="0fa26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fa26-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="0fa26-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fa26-106">Permissions</span></span>

<span data-ttu-id="0fa26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fa26-109">Permission type</span></span>      | <span data-ttu-id="0fa26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fa26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fa26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fa26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa26-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0fa26-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0fa26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fa26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa26-114">Not supported.</span></span>    |
|<span data-ttu-id="0fa26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fa26-115">Application</span></span> | <span data-ttu-id="0fa26-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa26-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fa26-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fa26-118">Optional query parameters</span></span>

<span data-ttu-id="0fa26-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0fa26-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="0fa26-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="0fa26-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="0fa26-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0fa26-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="0fa26-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="0fa26-123">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="0fa26-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="0fa26-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="0fa26-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="0fa26-125">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="0fa26-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="0fa26-126">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="0fa26-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="0fa26-127">Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário.</span><span class="sxs-lookup"><span data-stu-id="0fa26-127">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="0fa26-128">As seguintes propriedades só possuem suporte ao [recuperar um único usuário](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="0fa26-128">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fa26-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-129">Request headers</span></span>

| <span data-ttu-id="0fa26-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fa26-130">Header</span></span>        | <span data-ttu-id="0fa26-131">Valor</span><span class="sxs-lookup"><span data-stu-id="0fa26-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0fa26-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fa26-132">Authorization</span></span> | <span data-ttu-id="0fa26-133">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="0fa26-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="0fa26-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0fa26-134">ConsistencyLevel</span></span> | <span data-ttu-id="0fa26-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="0fa26-135">eventual.</span></span> <span data-ttu-id="0fa26-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="0fa26-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="0fa26-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa26-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-138">Request body</span></span>

<span data-ttu-id="0fa26-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fa26-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fa26-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-140">Response</span></span>

<span data-ttu-id="0fa26-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="0fa26-142">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="0fa26-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="0fa26-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0fa26-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="0fa26-144">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="0fa26-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-145">Request</span></span>

<span data-ttu-id="0fa26-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fa26-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa26-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="0fa26-148">C#</span><span class="sxs-lookup"><span data-stu-id="0fa26-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa26-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa26-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa26-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa26-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fa26-151">Java</span><span class="sxs-lookup"><span data-stu-id="0fa26-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0fa26-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-152">Response</span></span>

<span data-ttu-id="0fa26-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-153">The following is an example of the response.</span></span>

><span data-ttu-id="0fa26-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="0fa26-156">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="0fa26-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-157">Request</span></span>

<span data-ttu-id="0fa26-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-158">The following is an example of the request.</span></span>

><span data-ttu-id="0fa26-159">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="0fa26-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="0fa26-160">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="0fa26-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="0fa26-161">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="0fa26-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fa26-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa26-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="0fa26-163">C#</span><span class="sxs-lookup"><span data-stu-id="0fa26-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa26-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa26-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa26-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa26-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fa26-166">Java</span><span class="sxs-lookup"><span data-stu-id="0fa26-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0fa26-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-167">Response</span></span>

<span data-ttu-id="0fa26-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="0fa26-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="0fa26-171">Exemplo 3: obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="0fa26-171">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-172">Request</span></span>

<span data-ttu-id="0fa26-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0fa26-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-174">Response</span></span>

<span data-ttu-id="0fa26-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0fa26-176">Exemplo 4: utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0fa26-176">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-177">Request</span></span>

<span data-ttu-id="0fa26-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0fa26-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-179">Response</span></span>

<span data-ttu-id="0fa26-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-180">The following is an example of the response.</span></span>

><span data-ttu-id="0fa26-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="0fa26-183">Exemplo 5: utilize $filtro para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0fa26-183">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-184">Request</span></span>

<span data-ttu-id="0fa26-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fa26-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa26-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="0fa26-187">C#</span><span class="sxs-lookup"><span data-stu-id="0fa26-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa26-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa26-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa26-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa26-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fa26-190">Java</span><span class="sxs-lookup"><span data-stu-id="0fa26-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0fa26-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-191">Response</span></span>

<span data-ttu-id="0fa26-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-192">The following is an example of the response.</span></span>

><span data-ttu-id="0fa26-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="0fa26-195">Exemplo 6: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0fa26-195">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-196">Request</span></span>

<span data-ttu-id="0fa26-197">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0fa26-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-198">Response</span></span>

<span data-ttu-id="0fa26-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-199">The following is an example of the response.</span></span>

><span data-ttu-id="0fa26-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="0fa26-202">Exemplo 7: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras “wa”, ou as letras “para” incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0fa26-202">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0fa26-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa26-203">Request</span></span>

<span data-ttu-id="0fa26-204">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa26-204">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0fa26-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa26-205">Response</span></span>

<span data-ttu-id="0fa26-206">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa26-206">The following is an example of the response.</span></span>

> <span data-ttu-id="0fa26-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fa26-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
