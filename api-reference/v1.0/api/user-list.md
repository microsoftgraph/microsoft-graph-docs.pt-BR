---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9f573d50f498ba6bd022fce16e64496a5ace616c
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49030246"
---
# <a name="list-users"></a><span data-ttu-id="3b1a8-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="3b1a8-103">List users</span></span>

<span data-ttu-id="3b1a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b1a8-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3b1a8-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b1a8-106">Permissions</span></span>

<span data-ttu-id="3b1a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b1a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b1a8-109">Permission type</span></span>      | <span data-ttu-id="3b1a8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b1a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b1a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b1a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b1a8-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b1a8-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b1a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b1a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-114">Not supported.</span></span>    |
|<span data-ttu-id="3b1a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b1a8-115">Application</span></span> | <span data-ttu-id="3b1a8-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1a8-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b1a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b1a8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b1a8-118">Optional query parameters</span></span>

<span data-ttu-id="3b1a8-119">Este método suporta os parâmetros de consulta [OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, `$filter`, e `$select`.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="3b1a8-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="3b1a8-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3b1a8-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="3b1a8-123">Os parâmetros `$count` e `$search` não estão disponíveis no momento em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="3b1a8-124">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="3b1a8-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="3b1a8-125">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="3b1a8-126">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="3b1a8-127">Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-127">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="3b1a8-128">As seguintes propriedades só possuem suporte ao [recuperar um único usuário](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-128">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b1a8-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-129">Request headers</span></span>

| <span data-ttu-id="3b1a8-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b1a8-130">Header</span></span>        | <span data-ttu-id="3b1a8-131">Valor</span><span class="sxs-lookup"><span data-stu-id="3b1a8-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="3b1a8-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b1a8-132">Authorization</span></span> | <span data-ttu-id="3b1a8-133">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="3b1a8-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="3b1a8-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3b1a8-134">ConsistencyLevel</span></span> | <span data-ttu-id="3b1a8-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-135">eventual.</span></span> <span data-ttu-id="3b1a8-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="3b1a8-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b1a8-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-138">Request body</span></span>

<span data-ttu-id="3b1a8-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b1a8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-140">Response</span></span>

<span data-ttu-id="3b1a8-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="3b1a8-142">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="3b1a8-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="3b1a8-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b1a8-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="3b1a8-144">Exemplo 1: Obter todos os usuários</span><span class="sxs-lookup"><span data-stu-id="3b1a8-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-145">Request</span></span>

<span data-ttu-id="3b1a8-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-148">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-151">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-152">Response</span></span>

<span data-ttu-id="3b1a8-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-153">The following is an example of the response.</span></span>

><span data-ttu-id="3b1a8-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="3b1a8-156">Exemplo 2: Obter uma conta de usuário usando um nome de entrada</span><span class="sxs-lookup"><span data-stu-id="3b1a8-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-157">Request</span></span>

<span data-ttu-id="3b1a8-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-158">The following is an example of the request.</span></span>

><span data-ttu-id="3b1a8-159">**Observação:** Ao filtrar em **identidades**, você deve fornecer tanto **emissor** como **emissorAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-161">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-164">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-165">Response</span></span>

<span data-ttu-id="3b1a8-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-166">The following is an example of the response.</span></span> 

> <span data-ttu-id="3b1a8-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="3b1a8-169">Exemplo 3: Obter usuários incluindo o horário da última entrada</span><span class="sxs-lookup"><span data-stu-id="3b1a8-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-170">Request</span></span>

<span data-ttu-id="3b1a8-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-173">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-176">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-177">Response</span></span>

<span data-ttu-id="3b1a8-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-178">The following is an example of the response.</span></span>

><span data-ttu-id="3b1a8-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="3b1a8-181">Exemplo 4: listar o horário da última entrada de usuários com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="3b1a8-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-182">Request</span></span>

<span data-ttu-id="3b1a8-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-185">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-188">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-189">Response</span></span>

<span data-ttu-id="3b1a8-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-190">The following is an example of the response.</span></span> 

> <span data-ttu-id="3b1a8-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="3b1a8-193">Exemplo 5: listar o horário da última entrada dos usuários em um intervalo de tempo específico</span><span class="sxs-lookup"><span data-stu-id="3b1a8-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-194">Request</span></span>

<span data-ttu-id="3b1a8-195">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-195">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-197">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-200">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-201">Response</span></span>

<span data-ttu-id="3b1a8-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-202">The following is an example of the response.</span></span> 

> <span data-ttu-id="3b1a8-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="3b1a8-205">Exemplo 6: Obter apenas uma contagem de usuários</span><span class="sxs-lookup"><span data-stu-id="3b1a8-205">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-206">Request</span></span>

<span data-ttu-id="3b1a8-207">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-207">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-209">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-212">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-213">Response</span></span>

<span data-ttu-id="3b1a8-214">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-214">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3b1a8-215">Exemplo 7: Utilize $filter e $top para obter um usuário com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3b1a8-215">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-216">Request</span></span>

<span data-ttu-id="3b1a8-217">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-217">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-219">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-222">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-223">Response</span></span>

<span data-ttu-id="3b1a8-224">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-224">The following is an example of the response.</span></span>

><span data-ttu-id="3b1a8-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="3b1a8-227">Exemplo 8: Utilize $search para obter usuários com nomes de exibição que contenham as letras 'wa', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3b1a8-227">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-228">Request</span></span>

<span data-ttu-id="3b1a8-229">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-229">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b1a8-230">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1a8-230">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="3b1a8-231">C#</span><span class="sxs-lookup"><span data-stu-id="3b1a8-231">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1a8-232">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1a8-232">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1a8-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1a8-233">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1a8-234">Java</span><span class="sxs-lookup"><span data-stu-id="3b1a8-234">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-wa-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1a8-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-235">Response</span></span>

<span data-ttu-id="3b1a8-236">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-236">The following is an example of the response.</span></span>

><span data-ttu-id="3b1a8-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="3b1a8-239">Exemplo 9: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'wa', ou as letras para incluir uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3b1a8-239">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b1a8-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1a8-240">Request</span></span>

<span data-ttu-id="3b1a8-241">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-241">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b1a8-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1a8-242">Response</span></span>

<span data-ttu-id="3b1a8-243">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-243">The following is an example of the response.</span></span>

> <span data-ttu-id="3b1a8-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1a8-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
