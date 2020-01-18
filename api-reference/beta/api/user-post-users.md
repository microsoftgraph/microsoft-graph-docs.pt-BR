---
title: Criar usuário
description: Crie um novo usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e09525eaa1889a195d3a0d1c05793e6148d40ef1
ms.sourcegitcommit: bd0daf5c133ab29af9337a5edd3b8509fd2313d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41232039"
---
# <a name="create-user"></a><span data-ttu-id="75bb6-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="75bb6-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75bb6-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="75bb6-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="75bb6-108">Essa operação retorna, por padrão, apenas um subconjunto das propriedades de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-108">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="75bb6-109">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="75bb6-109">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="75bb6-110">Para obter propriedades não retornadas por padrão, execute uma [operação GET](user-get.md) e especifique as propriedades em uma opção de consulta do `$select` OData.</span><span class="sxs-lookup"><span data-stu-id="75bb6-110">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="75bb6-111">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="75bb6-111">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="75bb6-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="75bb6-112">Permissions</span></span>

<span data-ttu-id="75bb6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75bb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75bb6-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75bb6-115">Permission type</span></span>      | <span data-ttu-id="75bb6-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75bb6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75bb6-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75bb6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="75bb6-118">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75bb6-118">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="75bb6-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75bb6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75bb6-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75bb6-120">Not supported.</span></span>    |
|<span data-ttu-id="75bb6-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75bb6-121">Application</span></span> | <span data-ttu-id="75bb6-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75bb6-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75bb6-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75bb6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="75bb6-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75bb6-124">Request headers</span></span>
| <span data-ttu-id="75bb6-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75bb6-125">Header</span></span>       | <span data-ttu-id="75bb6-126">Valor</span><span class="sxs-lookup"><span data-stu-id="75bb6-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75bb6-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="75bb6-127">Authorization</span></span>  | <span data-ttu-id="75bb6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75bb6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75bb6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75bb6-130">Content-Type</span></span>  | <span data-ttu-id="75bb6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="75bb6-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75bb6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75bb6-132">Request body</span></span>

<span data-ttu-id="75bb6-133">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="75bb6-133">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="75bb6-134">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-134">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="75bb6-135">Se você estiver incluindo uma propriedade **Identities** para o usuário que você está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="75bb6-135">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="75bb6-136">Para uma [identidade de conta local B2C](../resources/objectidentity.md), somente **passwordProfile** é necessário e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="75bb6-136">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="75bb6-137">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="75bb6-137">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="75bb6-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75bb6-138">Parameter</span></span> | <span data-ttu-id="75bb6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="75bb6-139">Type</span></span> | <span data-ttu-id="75bb6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="75bb6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75bb6-141">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="75bb6-141">accountEnabled</span></span> |<span data-ttu-id="75bb6-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="75bb6-142">Boolean</span></span> |<span data-ttu-id="75bb6-143">True se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="75bb6-143">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="75bb6-144">displayName</span><span class="sxs-lookup"><span data-stu-id="75bb6-144">displayName</span></span> |<span data-ttu-id="75bb6-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75bb6-145">string</span></span> |<span data-ttu-id="75bb6-146">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-146">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="75bb6-147">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="75bb6-147">onPremisesImmutableId</span></span> |<span data-ttu-id="75bb6-148">string</span><span class="sxs-lookup"><span data-stu-id="75bb6-148">string</span></span> |<span data-ttu-id="75bb6-149">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-149">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="75bb6-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="75bb6-150">mailNickname</span></span> |<span data-ttu-id="75bb6-151">string</span><span class="sxs-lookup"><span data-stu-id="75bb6-151">string</span></span> |<span data-ttu-id="75bb6-152">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-152">The mail alias for the user.</span></span>|
|<span data-ttu-id="75bb6-153">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="75bb6-153">passwordProfile</span></span>|[<span data-ttu-id="75bb6-154">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="75bb6-154">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="75bb6-155">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="75bb6-155">The password profile for the user.</span></span>|
|<span data-ttu-id="75bb6-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75bb6-156">userPrincipalName</span></span> |<span data-ttu-id="75bb6-157">string</span><span class="sxs-lookup"><span data-stu-id="75bb6-157">string</span></span> |<span data-ttu-id="75bb6-158">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="75bb6-158">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="75bb6-159">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="75bb6-159">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="75bb6-160">Os usuários federados criados por meio dessa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="75bb6-160">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="75bb6-161">Para obter informações sobre como alterar isso, confira [exceções para tempos de vida do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="75bb6-161">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="75bb6-162">A adição de uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente não é permitida, a menos que o objeto **User** já contenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="75bb6-162">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="75bb6-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="75bb6-163">Response</span></span>

<span data-ttu-id="75bb6-164">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75bb6-164">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75bb6-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75bb6-165">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="75bb6-166">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="75bb6-166">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="75bb6-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75bb6-167">Request</span></span>
<span data-ttu-id="75bb6-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75bb6-168">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75bb6-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="75bb6-169">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="75bb6-170">C#</span><span class="sxs-lookup"><span data-stu-id="75bb6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75bb6-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75bb6-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75bb6-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75bb6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="75bb6-173">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="75bb6-173">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="75bb6-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="75bb6-174">Response</span></span>
<span data-ttu-id="75bb6-175">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75bb6-175">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="75bb6-176">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="75bb6-176">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75bb6-177">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75bb6-177">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="75bb6-178">Exemplo 2: criar um usuário com identidades sociais e de conta local</span><span class="sxs-lookup"><span data-stu-id="75bb6-178">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="75bb6-179">Crie um novo usuário, com uma identidade de conta local com um nome de entrada, um endereço de email como entrada e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="75bb6-179">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="75bb6-180">Este exemplo geralmente é usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="75bb6-180">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="75bb6-181">Para identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="75bb6-181">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="75bb6-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75bb6-182">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="75bb6-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="75bb6-183">HTTP</span></span>](#tab/http)
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
    "password": "password-value"
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75bb6-184">C#</span><span class="sxs-lookup"><span data-stu-id="75bb6-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75bb6-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75bb6-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75bb6-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75bb6-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="75bb6-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="75bb6-187">Response</span></span>

<span data-ttu-id="75bb6-188">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75bb6-188">Here is an example of the response.</span></span> 

> <span data-ttu-id="75bb6-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75bb6-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="75bb6-191">Confira também</span><span class="sxs-lookup"><span data-stu-id="75bb6-191">See also</span></span>

- [<span data-ttu-id="75bb6-192">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="75bb6-192">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="75bb6-193">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="75bb6-193">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="75bb6-194">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="75bb6-194">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
