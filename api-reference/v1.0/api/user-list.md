---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b9a598d994288859f1f8e2989c90cda7bab3300b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401370"
---
# <a name="list-users"></a><span data-ttu-id="ae091-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="ae091-103">List users</span></span>

<span data-ttu-id="ae091-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae091-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae091-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ae091-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae091-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae091-106">Permissions</span></span>

<span data-ttu-id="ae091-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae091-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae091-109">Permission type</span></span>      | <span data-ttu-id="ae091-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae091-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae091-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae091-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae091-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae091-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae091-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae091-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae091-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae091-114">Not supported.</span></span>    |
|<span data-ttu-id="ae091-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae091-115">Application</span></span> | <span data-ttu-id="ae091-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae091-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae091-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae091-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae091-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae091-118">Optional query parameters</span></span>

<span data-ttu-id="ae091-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ae091-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="ae091-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="ae091-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ae091-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="ae091-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ae091-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="ae091-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="ae091-123">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ae091-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="ae091-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="ae091-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> <span data-ttu-id="ae091-125">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="ae091-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="ae091-126">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="ae091-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="ae091-p104">Certas propriedades não podem ser retornadas em uma coleção de usuário. As seguintes propriedades terão suporte apenas [ao recuperar um único usuário:](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="ae091-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="ae091-129">As propriedades a seguir não têm suporte em contas pessoais da Microsoft e serão `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span><span class="sxs-lookup"><span data-stu-id="ae091-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae091-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-130">Request headers</span></span>

| <span data-ttu-id="ae091-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae091-131">Header</span></span>        | <span data-ttu-id="ae091-132">Valor</span><span class="sxs-lookup"><span data-stu-id="ae091-132">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="ae091-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae091-133">Authorization</span></span> | <span data-ttu-id="ae091-134">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="ae091-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ae091-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ae091-135">ConsistencyLevel</span></span> | <span data-ttu-id="ae091-136">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="ae091-136">eventual.</span></span> <span data-ttu-id="ae091-137">Este cabeçalho e `$count` são necessários ao usar `$search`, ou ao usar o `$filter` com o parâmetro de consulta `$orderby` ou `$filter` com o operador lógico `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="ae091-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="ae091-138">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="ae091-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae091-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-139">Request body</span></span>

<span data-ttu-id="ae091-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae091-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae091-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-141">Response</span></span>

<span data-ttu-id="ae091-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="ae091-143">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="ae091-143">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="ae091-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ae091-144">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="ae091-145">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="ae091-145">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-146">Request</span></span>

<span data-ttu-id="ae091-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae091-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae091-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="ae091-149">C#</span><span class="sxs-lookup"><span data-stu-id="ae091-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae091-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae091-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae091-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae091-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae091-152">Java</span><span class="sxs-lookup"><span data-stu-id="ae091-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae091-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-153">Response</span></span>

<span data-ttu-id="ae091-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-154">The following is an example of the response.</span></span>

><span data-ttu-id="ae091-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="ae091-156">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="ae091-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-157">Request</span></span>

<span data-ttu-id="ae091-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-158">The following is an example of the request.</span></span>

><span data-ttu-id="ae091-159">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="ae091-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="ae091-160">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="ae091-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="ae091-161">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="ae091-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae091-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae091-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="ae091-163">C#</span><span class="sxs-lookup"><span data-stu-id="ae091-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae091-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae091-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae091-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae091-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae091-166">Java</span><span class="sxs-lookup"><span data-stu-id="ae091-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae091-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-167">Response</span></span>

<span data-ttu-id="ae091-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="ae091-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="ae091-170">Exemplo 3: obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="ae091-170">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-171">Request</span></span>

<span data-ttu-id="ae091-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-172">The following is an example of the request.</span></span> <span data-ttu-id="ae091-173">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-173">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="ae091-174">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ae091-174">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ae091-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-175">Response</span></span>

<span data-ttu-id="ae091-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ae091-177">Exemplo 4: utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ae091-177">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-178">Request</span></span>

<span data-ttu-id="ae091-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-179">The following is an example of the request.</span></span> <span data-ttu-id="ae091-180">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ae091-180">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="ae091-181">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ae091-181">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ae091-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-182">Response</span></span>

<span data-ttu-id="ae091-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-183">The following is an example of the response.</span></span>

><span data-ttu-id="ae091-184">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-184">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="ae091-185">Exemplo 5: utilize $filtro para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae091-185">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-186">Request</span></span>

<span data-ttu-id="ae091-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-187">The following is an example of the request.</span></span> <span data-ttu-id="ae091-188">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`, e também usa o operador `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="ae091-188">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters, and also uses the `endsWith` operator.</span></span> <span data-ttu-id="ae091-189">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ae091-189">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


# <a name="http"></a>[<span data-ttu-id="ae091-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae091-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ae091-191">C#</span><span class="sxs-lookup"><span data-stu-id="ae091-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae091-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae091-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae091-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae091-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae091-194">Java</span><span class="sxs-lookup"><span data-stu-id="ae091-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae091-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-195">Response</span></span>

<span data-ttu-id="ae091-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-196">The following is an example of the response.</span></span>

><span data-ttu-id="ae091-197">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-197">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="ae091-198">Exemplo 6: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ae091-198">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-199">Request</span></span>

<span data-ttu-id="ae091-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-200">The following is an example of the request.</span></span> <span data-ttu-id="ae091-201">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-201">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="ae091-202">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ae091-202">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ae091-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-203">Response</span></span>

<span data-ttu-id="ae091-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-204">The following is an example of the response.</span></span>

><span data-ttu-id="ae091-205">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-205">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="ae091-206">Exemplo 7: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras “wa”, ou as letras “para” incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ae091-206">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-207">Request</span></span>

<span data-ttu-id="ae091-208">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-208">The following is an example of the request.</span></span> <span data-ttu-id="ae091-209">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-209">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="ae091-210">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ae091-210">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ae091-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-211">Response</span></span>

<span data-ttu-id="ae091-212">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-212">The following is an example of the response.</span></span>

> <span data-ttu-id="ae091-213">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ae091-213">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="ae091-214">Exemplo 8: Use $ filter para obter usuários que receberam uma licença específica</span><span class="sxs-lookup"><span data-stu-id="ae091-214">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="ae091-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae091-215">Request</span></span>

<span data-ttu-id="ae091-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae091-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="ae091-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae091-217">Response</span></span>

<span data-ttu-id="ae091-218">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae091-218">The following is an example of the response.</span></span>

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
