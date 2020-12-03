---
title: Criar usuário
description: Crie um novo usuário.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1bdbe81274b8769839cf97a5cf8025eea5e2f36e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523655"
---
# <a name="create-user"></a><span data-ttu-id="bf631-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="bf631-103">Create user</span></span>

<span data-ttu-id="bf631-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf631-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf631-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="bf631-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="bf631-109">Essa operação retorna, por padrão, apenas um subconjunto das propriedades de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-109">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="bf631-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="bf631-110">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="bf631-111">Para obter propriedades não retornadas por padrão, execute uma [operação GET](user-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="bf631-111">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="bf631-112">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="bf631-112">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf631-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf631-113">Permissions</span></span>

<span data-ttu-id="bf631-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf631-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf631-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf631-116">Permission type</span></span>      | <span data-ttu-id="bf631-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf631-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf631-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf631-118">Delegated (work or school account)</span></span> | <span data-ttu-id="bf631-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf631-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf631-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf631-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf631-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf631-121">Not supported.</span></span>    |
|<span data-ttu-id="bf631-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf631-122">Application</span></span> | <span data-ttu-id="bf631-123">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf631-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf631-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf631-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="bf631-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf631-125">Request headers</span></span>
| <span data-ttu-id="bf631-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf631-126">Header</span></span>       | <span data-ttu-id="bf631-127">Valor</span><span class="sxs-lookup"><span data-stu-id="bf631-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf631-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf631-128">Authorization</span></span>  | <span data-ttu-id="bf631-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf631-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf631-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf631-131">Content-Type</span></span>  | <span data-ttu-id="bf631-132">application/json</span><span class="sxs-lookup"><span data-stu-id="bf631-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf631-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf631-133">Request body</span></span>

<span data-ttu-id="bf631-134">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bf631-134">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="bf631-135">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-135">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="bf631-136">Se você estiver incluindo uma propriedade de **identidades** para o usuário que está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="bf631-136">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="bf631-137">Para obter uma [identidade de conta local B2C](../resources/objectidentity.md), só é necessário **passwordProfile** e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="bf631-137">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="bf631-138">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="bf631-138">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="bf631-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bf631-139">Parameter</span></span> | <span data-ttu-id="bf631-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf631-140">Type</span></span> | <span data-ttu-id="bf631-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf631-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf631-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="bf631-142">accountEnabled</span></span> |<span data-ttu-id="bf631-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf631-143">Boolean</span></span> |<span data-ttu-id="bf631-144">True se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="bf631-144">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="bf631-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bf631-145">displayName</span></span> |<span data-ttu-id="bf631-146">string</span><span class="sxs-lookup"><span data-stu-id="bf631-146">string</span></span> |<span data-ttu-id="bf631-147">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-147">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="bf631-148">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="bf631-148">onPremisesImmutableId</span></span> |<span data-ttu-id="bf631-149">string</span><span class="sxs-lookup"><span data-stu-id="bf631-149">string</span></span> |<span data-ttu-id="bf631-150">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-150">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="bf631-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bf631-151">mailNickname</span></span> |<span data-ttu-id="bf631-152">string</span><span class="sxs-lookup"><span data-stu-id="bf631-152">string</span></span> |<span data-ttu-id="bf631-153">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-153">The mail alias for the user.</span></span>|
|<span data-ttu-id="bf631-154">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="bf631-154">passwordProfile</span></span>|[<span data-ttu-id="bf631-155">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="bf631-155">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="bf631-156">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf631-156">The password profile for the user.</span></span>|
|<span data-ttu-id="bf631-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bf631-157">userPrincipalName</span></span> |<span data-ttu-id="bf631-158">string</span><span class="sxs-lookup"><span data-stu-id="bf631-158">string</span></span> |<span data-ttu-id="bf631-159">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="bf631-159">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="bf631-160">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="bf631-160">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="bf631-161">Os usuários federados criados por meio dessa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="bf631-161">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="bf631-162">Para obter informações sobre como alterar isso, confira [exceções para tempos de vida do token](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="bf631-162">For information about how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="bf631-163">A adição de uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente não é permitida, a menos que o objeto **User** já contenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="bf631-163">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="bf631-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf631-164">Response</span></span>

<span data-ttu-id="bf631-165">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf631-165">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf631-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf631-166">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="bf631-167">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="bf631-167">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="bf631-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf631-168">Request</span></span>
<span data-ttu-id="bf631-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf631-169">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf631-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf631-170">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="c"></a>[<span data-ttu-id="bf631-171">C#</span><span class="sxs-lookup"><span data-stu-id="bf631-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf631-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf631-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf631-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf631-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf631-174">Java</span><span class="sxs-lookup"><span data-stu-id="bf631-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bf631-175">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bf631-175">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bf631-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf631-176">Response</span></span>
<span data-ttu-id="bf631-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf631-177">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="bf631-178">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf631-178">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bf631-179">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf631-179">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="bf631-180">Exemplo 2: criar um usuário com identidades de conta social e local</span><span class="sxs-lookup"><span data-stu-id="bf631-180">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="bf631-181">Crie um novo usuário, com uma identidade de conta local, com um nome de logon, um endereço de email como logon e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="bf631-181">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="bf631-182">Esse exemplo é geralmente usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="bf631-182">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="bf631-183">Para as identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="bf631-183">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="bf631-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf631-184">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf631-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf631-185">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="c"></a>[<span data-ttu-id="bf631-186">C#</span><span class="sxs-lookup"><span data-stu-id="bf631-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf631-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf631-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf631-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf631-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf631-189">Java</span><span class="sxs-lookup"><span data-stu-id="bf631-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bf631-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf631-190">Response</span></span>

<span data-ttu-id="bf631-191">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf631-191">Here is an example of the response.</span></span> 

> <span data-ttu-id="bf631-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf631-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
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

## <a name="see-also"></a><span data-ttu-id="bf631-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf631-194">See also</span></span>

- [<span data-ttu-id="bf631-195">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="bf631-195">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bf631-196">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="bf631-196">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bf631-197">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="bf631-197">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
