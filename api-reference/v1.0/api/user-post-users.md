---
title: Criar Usuário
description: Usar esta API para criar um novo Usuário.
author: krbain
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6caceda1131af15fd593167b3235b4c6a25b2e58
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081320"
---
# <a name="create-user"></a><span data-ttu-id="21e25-103">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="21e25-103">Create User</span></span>

<span data-ttu-id="21e25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21e25-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21e25-105">Create a new [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="21e25-105">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="21e25-106">The request body contains the user to create.</span><span class="sxs-lookup"><span data-stu-id="21e25-106">The request body contains the user to create.</span></span> <span data-ttu-id="21e25-107">At a minimum, you must specify the required properties for the user.</span><span class="sxs-lookup"><span data-stu-id="21e25-107">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="21e25-108">You can optionally specify any other writable properties.</span><span class="sxs-lookup"><span data-stu-id="21e25-108">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="21e25-109">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="21e25-109">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="21e25-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="21e25-110">Permissions</span></span>

<span data-ttu-id="21e25-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="21e25-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="21e25-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e25-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21e25-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21e25-113">Permission type</span></span>      | <span data-ttu-id="21e25-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21e25-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21e25-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21e25-115">Delegated (work or school account)</span></span> | <span data-ttu-id="21e25-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21e25-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21e25-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21e25-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e25-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21e25-118">Not supported.</span></span>    |
|<span data-ttu-id="21e25-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21e25-119">Application</span></span> | <span data-ttu-id="21e25-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e25-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21e25-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21e25-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="21e25-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21e25-122">Request headers</span></span>

| <span data-ttu-id="21e25-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21e25-123">Header</span></span>       | <span data-ttu-id="21e25-124">Valor</span><span class="sxs-lookup"><span data-stu-id="21e25-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21e25-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="21e25-125">Authorization</span></span>  | <span data-ttu-id="21e25-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="21e25-126">Bearer {token}.</span></span> <span data-ttu-id="21e25-127">Required.</span><span class="sxs-lookup"><span data-stu-id="21e25-127">Required.</span></span>  |
| <span data-ttu-id="21e25-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21e25-128">Content-Type</span></span>  | <span data-ttu-id="21e25-129">application/json</span><span class="sxs-lookup"><span data-stu-id="21e25-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21e25-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21e25-130">Request body</span></span>

<span data-ttu-id="21e25-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="21e25-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="21e25-132">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="21e25-132">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="21e25-133">Se você estiver incluindo uma propriedade de **identidades** para o usuário que está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="21e25-133">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="21e25-134">Para obter uma [identidade de conta local B2C](../resources/objectidentity.md), só é necessário **passwordProfile** e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="21e25-134">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="21e25-135">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="21e25-135">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="21e25-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="21e25-136">Parameter</span></span> | <span data-ttu-id="21e25-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="21e25-137">Type</span></span> | <span data-ttu-id="21e25-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e25-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21e25-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="21e25-139">accountEnabled</span></span> |<span data-ttu-id="21e25-140">booliano</span><span class="sxs-lookup"><span data-stu-id="21e25-140">boolean</span></span> |<span data-ttu-id="21e25-141">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="21e25-141">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="21e25-142">displayName</span><span class="sxs-lookup"><span data-stu-id="21e25-142">displayName</span></span> |<span data-ttu-id="21e25-143">string</span><span class="sxs-lookup"><span data-stu-id="21e25-143">string</span></span> |<span data-ttu-id="21e25-144">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e25-144">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="21e25-145">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="21e25-145">onPremisesImmutableId</span></span> |<span data-ttu-id="21e25-146">string</span><span class="sxs-lookup"><span data-stu-id="21e25-146">string</span></span> |<span data-ttu-id="21e25-147">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e25-147">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="21e25-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="21e25-148">mailNickname</span></span> |<span data-ttu-id="21e25-149">string</span><span class="sxs-lookup"><span data-stu-id="21e25-149">string</span></span> |<span data-ttu-id="21e25-150">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e25-150">The mail alias for the user.</span></span>|
|<span data-ttu-id="21e25-151">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="21e25-151">passwordProfile</span></span>|[<span data-ttu-id="21e25-152">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="21e25-152">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="21e25-153">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e25-153">The password profile for the user.</span></span>|
|<span data-ttu-id="21e25-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21e25-154">userPrincipalName</span></span> |<span data-ttu-id="21e25-155">string</span><span class="sxs-lookup"><span data-stu-id="21e25-155">string</span></span> |<span data-ttu-id="21e25-156">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="21e25-156">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="21e25-157">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="21e25-157">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="21e25-158">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="21e25-158">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="21e25-159">Para obter mais informações sobre como alterar isso, confira [exceções para vidas úteis de token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="21e25-159">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="21e25-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e25-160">Response</span></span>

<span data-ttu-id="21e25-161">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21e25-161">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e25-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21e25-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="21e25-163">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="21e25-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="21e25-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21e25-164">Request</span></span>

<span data-ttu-id="21e25-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21e25-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21e25-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="21e25-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="21e25-167">C#</span><span class="sxs-lookup"><span data-stu-id="21e25-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21e25-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21e25-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21e25-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21e25-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21e25-170">Java</span><span class="sxs-lookup"><span data-stu-id="21e25-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="21e25-171">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="21e25-171">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="21e25-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e25-172">Response</span></span>

<span data-ttu-id="21e25-173">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="21e25-173">Here is an example of the response.</span></span> <span data-ttu-id="21e25-174">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="21e25-174">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21e25-175">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="21e25-175">All of the properties will be returned from an actual call.</span></span>
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
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="21e25-176">Exemplo 2: criar um usuário com identidades de conta social e local</span><span class="sxs-lookup"><span data-stu-id="21e25-176">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="21e25-177">Crie um novo usuário, com uma identidade de conta local, com um nome de logon, um endereço de email como logon e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="21e25-177">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="21e25-178">Esse exemplo é geralmente usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="21e25-178">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="21e25-179">Para as identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="21e25-179">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="21e25-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21e25-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="21e25-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="21e25-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="21e25-182">C#</span><span class="sxs-lookup"><span data-stu-id="21e25-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21e25-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21e25-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21e25-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21e25-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21e25-185">Java</span><span class="sxs-lookup"><span data-stu-id="21e25-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21e25-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e25-186">Response</span></span>

<span data-ttu-id="21e25-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21e25-187">Here is an example of the response.</span></span> 

> <span data-ttu-id="21e25-188">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="21e25-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21e25-189">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="21e25-189">All the properties will be returned from an actual call.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="21e25-190">Confira também</span><span class="sxs-lookup"><span data-stu-id="21e25-190">See also</span></span>

- [<span data-ttu-id="21e25-191">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="21e25-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="21e25-192">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="21e25-192">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)

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
