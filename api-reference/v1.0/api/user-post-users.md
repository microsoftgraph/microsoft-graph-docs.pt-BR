---
title: Criar Usuário
description: Usar esta API para criar um novo Usuário.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d0d3501916a2c2a2f5a08881c8e6be8ba4384823
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053759"
---
# <a name="create-user"></a><span data-ttu-id="725b9-103">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="725b9-103">Create User</span></span>

<span data-ttu-id="725b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="725b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="725b9-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="725b9-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="725b9-109">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="725b9-109">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="725b9-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="725b9-110">Permissions</span></span>

<span data-ttu-id="725b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="725b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="725b9-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="725b9-113">Permission type</span></span>      | <span data-ttu-id="725b9-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="725b9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="725b9-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="725b9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="725b9-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="725b9-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="725b9-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="725b9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="725b9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="725b9-118">Not supported.</span></span>    |
|<span data-ttu-id="725b9-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="725b9-119">Application</span></span> | <span data-ttu-id="725b9-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725b9-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="725b9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="725b9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="725b9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="725b9-122">Request headers</span></span>

| <span data-ttu-id="725b9-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="725b9-123">Header</span></span>       | <span data-ttu-id="725b9-124">Valor</span><span class="sxs-lookup"><span data-stu-id="725b9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="725b9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="725b9-125">Authorization</span></span>  | <span data-ttu-id="725b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="725b9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="725b9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="725b9-128">Content-Type</span></span>  | <span data-ttu-id="725b9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="725b9-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="725b9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="725b9-130">Request body</span></span>

<span data-ttu-id="725b9-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="725b9-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="725b9-132">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="725b9-132">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="725b9-133">Se você estiver incluindo uma propriedade de **identidades** para o usuário que está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="725b9-133">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="725b9-134">Para obter uma [identidade de conta local B2C](../resources/objectidentity.md), só é necessário **passwordProfile** e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="725b9-134">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="725b9-135">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="725b9-135">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="725b9-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="725b9-136">Parameter</span></span> | <span data-ttu-id="725b9-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="725b9-137">Type</span></span> | <span data-ttu-id="725b9-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="725b9-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="725b9-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="725b9-139">accountEnabled</span></span> |<span data-ttu-id="725b9-140">booliano</span><span class="sxs-lookup"><span data-stu-id="725b9-140">boolean</span></span> |<span data-ttu-id="725b9-141">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="725b9-141">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="725b9-142">displayName</span><span class="sxs-lookup"><span data-stu-id="725b9-142">displayName</span></span> |<span data-ttu-id="725b9-143">string</span><span class="sxs-lookup"><span data-stu-id="725b9-143">string</span></span> |<span data-ttu-id="725b9-144">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="725b9-144">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="725b9-145">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="725b9-145">onPremisesImmutableId</span></span> |<span data-ttu-id="725b9-146">string</span><span class="sxs-lookup"><span data-stu-id="725b9-146">string</span></span> |<span data-ttu-id="725b9-147">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="725b9-147">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="725b9-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="725b9-148">mailNickname</span></span> |<span data-ttu-id="725b9-149">string</span><span class="sxs-lookup"><span data-stu-id="725b9-149">string</span></span> |<span data-ttu-id="725b9-150">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="725b9-150">The mail alias for the user.</span></span>|
|<span data-ttu-id="725b9-151">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="725b9-151">passwordProfile</span></span>|[<span data-ttu-id="725b9-152">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="725b9-152">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="725b9-153">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="725b9-153">The password profile for the user.</span></span>|
|<span data-ttu-id="725b9-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="725b9-154">userPrincipalName</span></span> |<span data-ttu-id="725b9-155">string</span><span class="sxs-lookup"><span data-stu-id="725b9-155">string</span></span> |<span data-ttu-id="725b9-156">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="725b9-156">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="725b9-157">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="725b9-157">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="725b9-158">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="725b9-158">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="725b9-159">Para obter mais informações sobre como alterar isso, confira [exceções para vidas úteis de token](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="725b9-159">For more information on how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="725b9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="725b9-160">Response</span></span>

<span data-ttu-id="725b9-161">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="725b9-161">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="725b9-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="725b9-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="725b9-163">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="725b9-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="725b9-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="725b9-164">Request</span></span>

<span data-ttu-id="725b9-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="725b9-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="725b9-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="725b9-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "Adele Vance",
  "mailNickname": "AdeleV",
  "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="725b9-167">C#</span><span class="sxs-lookup"><span data-stu-id="725b9-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="725b9-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="725b9-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="725b9-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="725b9-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="725b9-170">Java</span><span class="sxs-lookup"><span data-stu-id="725b9-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="725b9-171">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="725b9-171">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="725b9-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="725b9-172">Response</span></span>

<span data-ttu-id="725b9-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="725b9-173">Here is an example of the response.</span></span> <span data-ttu-id="725b9-174">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="725b9-174">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd",
    "businessPhones": [],
    "displayName": "Adele Vance",
    "givenName": "Adele",
    "jobTitle": "Product Marketing Manager",
    "mail": "AdeleV@contoso.onmicrosoft.com",
    "mobilePhone": "+1 425 555 0109",
    "officeLocation": "18/2111",
    "preferredLanguage": "en-US",
    "surname": "Vance",
    "userPrincipalName": "AdeleV@contoso.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="725b9-175">Exemplo 2: criar um usuário com identidades de conta social e local</span><span class="sxs-lookup"><span data-stu-id="725b9-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="725b9-176">Crie um novo usuário, com uma identidade de conta local, com um nome de logon, um endereço de email como logon e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="725b9-176">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="725b9-177">Esse exemplo é geralmente usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="725b9-177">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="725b9-178">Para as identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="725b9-178">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="725b9-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="725b9-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="725b9-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="725b9-180">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "displayName": "John Smith",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    "password": "password-value",
    "forceChangePasswordNextSignIn": false
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="c"></a>[<span data-ttu-id="725b9-181">C#</span><span class="sxs-lookup"><span data-stu-id="725b9-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="725b9-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="725b9-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="725b9-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="725b9-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="725b9-184">Java</span><span class="sxs-lookup"><span data-stu-id="725b9-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="725b9-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="725b9-185">Response</span></span>

<span data-ttu-id="725b9-186">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="725b9-186">Here is an example of the response.</span></span> 

> <span data-ttu-id="725b9-187">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="725b9-187">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "displayName": "John Smith",
  "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordPolicies": "DisablePasswordExpiration"
}
```
## <a name="see-also"></a><span data-ttu-id="725b9-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="725b9-188">See also</span></span>

- [<span data-ttu-id="725b9-189">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="725b9-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="725b9-190">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="725b9-190">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
