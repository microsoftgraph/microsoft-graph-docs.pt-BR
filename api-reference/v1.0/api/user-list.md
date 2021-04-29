---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 79c60a53edf8d5c105d0a12a4ce53514e6dc8cb2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52033654"
---
# <a name="list-users"></a><span data-ttu-id="997d6-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="997d6-103">List users</span></span>

<span data-ttu-id="997d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="997d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="997d6-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="997d6-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="997d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="997d6-106">Permissions</span></span>

<span data-ttu-id="997d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="997d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="997d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="997d6-109">Permission type</span></span>      | <span data-ttu-id="997d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="997d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="997d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="997d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="997d6-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="997d6-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="997d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="997d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="997d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="997d6-114">Not supported.</span></span>    |
|<span data-ttu-id="997d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="997d6-115">Application</span></span> | <span data-ttu-id="997d6-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997d6-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="997d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="997d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="997d6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="997d6-118">Optional query parameters</span></span>

<span data-ttu-id="997d6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="997d6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="997d6-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="997d6-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="997d6-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="997d6-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="997d6-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="997d6-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="997d6-123">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="997d6-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="997d6-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="997d6-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="997d6-125">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="997d6-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="997d6-126">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="997d6-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="997d6-p104">Certas propriedades não podem ser retornadas em uma coleção de usuário. As seguintes propriedades são suportadas apenas [ao recuperar um único usuário:](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="997d6-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="997d6-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-129">Request headers</span></span>

| <span data-ttu-id="997d6-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="997d6-130">Header</span></span>        | <span data-ttu-id="997d6-131">Valor</span><span class="sxs-lookup"><span data-stu-id="997d6-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="997d6-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="997d6-132">Authorization</span></span> | <span data-ttu-id="997d6-133">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="997d6-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="997d6-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="997d6-134">ConsistencyLevel</span></span> | <span data-ttu-id="997d6-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="997d6-135">eventual.</span></span> <span data-ttu-id="997d6-136">Este cabeçalho e `$count` são necessários ao usar `$search`, ou ao usar o `$filter` com o parâmetro de consulta `$orderby` ou `$filter` com o operador lógico `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="997d6-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="997d6-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="997d6-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="997d6-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-138">Request body</span></span>

<span data-ttu-id="997d6-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="997d6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="997d6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-140">Response</span></span>

<span data-ttu-id="997d6-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="997d6-142">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="997d6-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="997d6-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="997d6-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="997d6-144">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="997d6-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-145">Request</span></span>

<span data-ttu-id="997d6-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="997d6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="997d6-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="997d6-148">C#</span><span class="sxs-lookup"><span data-stu-id="997d6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="997d6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="997d6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="997d6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="997d6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="997d6-151">Java</span><span class="sxs-lookup"><span data-stu-id="997d6-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="997d6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-152">Response</span></span>

<span data-ttu-id="997d6-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-153">The following is an example of the response.</span></span>

><span data-ttu-id="997d6-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="997d6-155">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="997d6-155">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-156">Request</span></span>

<span data-ttu-id="997d6-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-157">The following is an example of the request.</span></span>

><span data-ttu-id="997d6-158">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="997d6-158">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="997d6-159">O valor de **issuerAssignedId** deve ser o endereço de email da conta do usuário, não o nome de usuário principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="997d6-159">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="997d6-160">Se um UPN for usado, a resposta será uma lista em branco.</span><span class="sxs-lookup"><span data-stu-id="997d6-160">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="997d6-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="997d6-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="997d6-162">C#</span><span class="sxs-lookup"><span data-stu-id="997d6-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="997d6-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="997d6-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="997d6-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="997d6-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="997d6-165">Java</span><span class="sxs-lookup"><span data-stu-id="997d6-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="997d6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-166">Response</span></span>

<span data-ttu-id="997d6-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-167">The following is an example of the response.</span></span> 

> <span data-ttu-id="997d6-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="997d6-169">Exemplo 3: obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="997d6-169">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-170">Request</span></span>

<span data-ttu-id="997d6-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="997d6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-172">Response</span></span>

<span data-ttu-id="997d6-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-173">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="997d6-174">Exemplo 4: utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="997d6-174">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-175">Request</span></span>

<span data-ttu-id="997d6-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="997d6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-177">Response</span></span>

<span data-ttu-id="997d6-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-178">The following is an example of the response.</span></span>

><span data-ttu-id="997d6-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="997d6-180">Exemplo 5: utilize $filtro para obter todos os usuários com um email que termina com “a@contoso.com”, incluindo uma contagem de objetos retornados, com os resultados pedidos por userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="997d6-180">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-181">Request</span></span>

<span data-ttu-id="997d6-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="997d6-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="997d6-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="997d6-184">C#</span><span class="sxs-lookup"><span data-stu-id="997d6-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="997d6-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="997d6-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="997d6-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="997d6-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="997d6-187">Java</span><span class="sxs-lookup"><span data-stu-id="997d6-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="997d6-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-188">Response</span></span>

<span data-ttu-id="997d6-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-189">The following is an example of the response.</span></span>

><span data-ttu-id="997d6-190">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-190">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="997d6-191">Exemplo 6: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="997d6-191">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-192">Request</span></span>

<span data-ttu-id="997d6-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="997d6-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-194">Response</span></span>

<span data-ttu-id="997d6-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-195">The following is an example of the response.</span></span>

><span data-ttu-id="997d6-196">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="997d6-197">Exemplo 7: utilize $pesquisa para obter usuários com nomes de exibição que contenham as letras “wa”, ou as letras “para” incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="997d6-197">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-198">Request</span></span>

<span data-ttu-id="997d6-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-199">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="997d6-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-200">Response</span></span>

<span data-ttu-id="997d6-201">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-201">The following is an example of the response.</span></span>

> <span data-ttu-id="997d6-202">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="997d6-202">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="997d6-203">Exemplo 8: Use $ filter para obter usuários que receberam uma licença específica</span><span class="sxs-lookup"><span data-stu-id="997d6-203">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="997d6-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997d6-204">Request</span></span>

<span data-ttu-id="997d6-205">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="997d6-205">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="997d6-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="997d6-206">Response</span></span>

<span data-ttu-id="997d6-207">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="997d6-207">The following is an example of the response.</span></span>

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
