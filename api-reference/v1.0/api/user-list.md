---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d20e60757fce6b2981ce4db1d06ffe29930e3539
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634872"
---
# <a name="list-users"></a><span data-ttu-id="1c810-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="1c810-103">List users</span></span>

<span data-ttu-id="1c810-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c810-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c810-105">Recupere uma lista de objetos [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1c810-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c810-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c810-106">Permissions</span></span>

<span data-ttu-id="1c810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c810-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c810-109">Permission type</span></span>      | <span data-ttu-id="1c810-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c810-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c810-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c810-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c810-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c810-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c810-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c810-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c810-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c810-114">Not supported.</span></span>    |
|<span data-ttu-id="1c810-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c810-115">Application</span></span> | <span data-ttu-id="1c810-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c810-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c810-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c810-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c810-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c810-118">Optional query parameters</span></span>

<span data-ttu-id="1c810-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c810-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="1c810-120">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** e **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="1c810-120">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="1c810-121">Para retornar um conjunto de propriedades alternativas, especifique o conjunto desejado de propriedades do [usuário](../resources/user.md) usando o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="1c810-121">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="1c810-122">Por exemplo, para retornar**displayName**, **givenName** e **postalCode**, adicione o seguinte à sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="1c810-122">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="1c810-123">Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário.</span><span class="sxs-lookup"><span data-stu-id="1c810-123">Certain properties cannot be returned within a user collection.</span></span> <span data-ttu-id="1c810-124">As seguintes propriedades só possuem suporte ao [recuperar um único usuário](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="1c810-124">The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c810-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c810-125">Request headers</span></span>

| <span data-ttu-id="1c810-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c810-126">Header</span></span>        | <span data-ttu-id="1c810-127">Valor</span><span class="sxs-lookup"><span data-stu-id="1c810-127">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="1c810-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c810-128">Authorization</span></span> | <span data-ttu-id="1c810-129">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="1c810-129">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c810-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c810-130">Request body</span></span>

<span data-ttu-id="1c810-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c810-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c810-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c810-132">Response</span></span>

<span data-ttu-id="1c810-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c810-133">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="1c810-134">Se uma coleção grande de usuários for retornada, você poderá usar a [paginação no seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1c810-134">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="1c810-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c810-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="1c810-136">Exemplo 1: Solicitação de usuários padrão</span><span class="sxs-lookup"><span data-stu-id="1c810-136">Example 1: Standard users request</span></span>

<span data-ttu-id="1c810-137">Por padrão, apenas um conjunto limitado de propriedades é retornado (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="1c810-137">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span></span> <span data-ttu-id="1c810-138">Este exemplo ilustra a solicitação padrão e a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c810-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="1c810-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c810-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1c810-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c810-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="1c810-141">C#</span><span class="sxs-lookup"><span data-stu-id="1c810-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c810-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c810-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c810-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c810-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c810-144">Java</span><span class="sxs-lookup"><span data-stu-id="1c810-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c810-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c810-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="1c810-146">Exemplo 2: Solicitação de usuários usando $select</span><span class="sxs-lookup"><span data-stu-id="1c810-146">Example 2: Users request using $select</span></span>

<span data-ttu-id="1c810-147">Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="1c810-147">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="1c810-148">Por exemplo, para retornar **displayName**, **givenName** e **postalCode**, você incluiria o seguinte na sua consulta `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="1c810-148">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

##### <a name="request"></a><span data-ttu-id="1c810-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c810-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1c810-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c810-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="1c810-151">C#</span><span class="sxs-lookup"><span data-stu-id="1c810-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c810-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c810-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c810-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c810-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c810-154">Java</span><span class="sxs-lookup"><span data-stu-id="1c810-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c810-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c810-155">Response</span></span>

<span data-ttu-id="1c810-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1c810-156">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

### <a name="example-3-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="1c810-157">Exemplo 3: localizar uma conta de usuário usando o nome de logon</span><span class="sxs-lookup"><span data-stu-id="1c810-157">Example 3: Find a user account using a sign-in name</span></span>

<span data-ttu-id="1c810-158">Encontrar uma conta de usuário em um locatário B2C usando um nome de entrada (também conhecido como conta local).</span><span class="sxs-lookup"><span data-stu-id="1c810-158">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="1c810-159">Essa solicitação pode ser usada por um suporte técnico para encontrar uma conta de usuário do cliente, em um locatário B2C (neste exemplo, o locatário B2C é contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="1c810-159">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="1c810-160">Ao filtrar por **identidades**, você deve fornecer o **emissor** e **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="1c810-160">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="1c810-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c810-161">Request</span></span>

<span data-ttu-id="1c810-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c810-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c810-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c810-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="1c810-164">C#</span><span class="sxs-lookup"><span data-stu-id="1c810-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c810-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c810-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c810-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c810-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c810-167">Java</span><span class="sxs-lookup"><span data-stu-id="1c810-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="1c810-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c810-168">Response</span></span>

<span data-ttu-id="1c810-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c810-169">The following is an example of the response.</span></span> 
> <span data-ttu-id="1c810-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c810-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
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
