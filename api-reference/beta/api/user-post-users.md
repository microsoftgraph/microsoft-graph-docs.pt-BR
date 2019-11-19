---
title: Criar usuário
description: Crie um novo usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b4a34190fd2ec6d61cdfb03e004e7673d60cddb
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703739"
---
# <a name="create-user"></a><span data-ttu-id="7d1ea-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="7d1ea-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d1ea-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="7d1ea-108">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d1ea-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d1ea-109">Permissions</span></span>

<span data-ttu-id="7d1ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d1ea-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d1ea-112">Permission type</span></span>      | <span data-ttu-id="7d1ea-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d1ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d1ea-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d1ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7d1ea-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d1ea-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d1ea-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d1ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d1ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-117">Not supported.</span></span>    |
|<span data-ttu-id="7d1ea-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d1ea-118">Application</span></span> | <span data-ttu-id="7d1ea-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d1ea-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d1ea-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1ea-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="7d1ea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d1ea-121">Request headers</span></span>
| <span data-ttu-id="7d1ea-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d1ea-122">Header</span></span>       | <span data-ttu-id="7d1ea-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7d1ea-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d1ea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d1ea-124">Authorization</span></span>  | <span data-ttu-id="7d1ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7d1ea-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d1ea-127">Content-Type</span></span>  | <span data-ttu-id="7d1ea-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d1ea-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d1ea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d1ea-129">Request body</span></span>

<span data-ttu-id="7d1ea-130">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="7d1ea-131">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-131">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="7d1ea-132">Se você estiver incluindo uma propriedade **Identities** para o usuário que você está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-132">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="7d1ea-133">Para uma [identidade de conta local B2C](../resources/objectidentity.md), somente **passwordProfile** é necessário e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-133">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="7d1ea-134">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-134">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="7d1ea-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d1ea-135">Parameter</span></span> | <span data-ttu-id="7d1ea-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d1ea-136">Type</span></span> | <span data-ttu-id="7d1ea-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d1ea-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d1ea-138">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7d1ea-138">accountEnabled</span></span> |<span data-ttu-id="7d1ea-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d1ea-139">Boolean</span></span> |<span data-ttu-id="7d1ea-140">True se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-140">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="7d1ea-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7d1ea-141">displayName</span></span> |<span data-ttu-id="7d1ea-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1ea-142">string</span></span> |<span data-ttu-id="7d1ea-143">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-143">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="7d1ea-144">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="7d1ea-144">onPremisesImmutableId</span></span> |<span data-ttu-id="7d1ea-145">string</span><span class="sxs-lookup"><span data-stu-id="7d1ea-145">string</span></span> |<span data-ttu-id="7d1ea-146">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-146">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="7d1ea-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7d1ea-147">mailNickname</span></span> |<span data-ttu-id="7d1ea-148">string</span><span class="sxs-lookup"><span data-stu-id="7d1ea-148">string</span></span> |<span data-ttu-id="7d1ea-149">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-149">The mail alias for the user.</span></span>|
|<span data-ttu-id="7d1ea-150">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="7d1ea-150">passwordProfile</span></span>|[<span data-ttu-id="7d1ea-151">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="7d1ea-151">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="7d1ea-152">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-152">The password profile for the user.</span></span>|
|<span data-ttu-id="7d1ea-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d1ea-153">userPrincipalName</span></span> |<span data-ttu-id="7d1ea-154">string</span><span class="sxs-lookup"><span data-stu-id="7d1ea-154">string</span></span> |<span data-ttu-id="7d1ea-155">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-155">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="7d1ea-156">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-156">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="7d1ea-157">Os usuários federados criados por meio dessa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-157">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="7d1ea-158">Para obter informações sobre como alterar isso, confira [exceções para tempos de vida do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-158">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="7d1ea-159">A adição de uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente não é permitida, a menos que o objeto **User** já contenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-159">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="7d1ea-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d1ea-160">Response</span></span>

<span data-ttu-id="7d1ea-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-161">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d1ea-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d1ea-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="7d1ea-163">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="7d1ea-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="7d1ea-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d1ea-164">Request</span></span>
<span data-ttu-id="7d1ea-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-165">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7d1ea-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1ea-166">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d1ea-167">C#</span><span class="sxs-lookup"><span data-stu-id="7d1ea-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d1ea-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d1ea-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d1ea-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d1ea-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7d1ea-170">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7d1ea-170">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7d1ea-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d1ea-171">Response</span></span>
<span data-ttu-id="7d1ea-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-172">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="7d1ea-173">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-173">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d1ea-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-174">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="7d1ea-175">Exemplo 2: criar um usuário com identidades sociais e de conta local</span><span class="sxs-lookup"><span data-stu-id="7d1ea-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="7d1ea-176">Crie um novo usuário, com uma identidade de conta local com um nome de entrada, um endereço de email como entrada e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-176">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="7d1ea-177">Este exemplo geralmente é usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-177">This example is typically used for migration scenarios in B2C tenants.</span></span>  

[!NOTE] 
<span data-ttu-id="7d1ea-178">Para identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-178">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="7d1ea-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d1ea-179">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7d1ea-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1ea-180">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d1ea-181">C#</span><span class="sxs-lookup"><span data-stu-id="7d1ea-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d1ea-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d1ea-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d1ea-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d1ea-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d1ea-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d1ea-184">Response</span></span>

<span data-ttu-id="7d1ea-185">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-185">Here is an example of the response.</span></span> 

> <span data-ttu-id="7d1ea-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d1ea-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7d1ea-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="7d1ea-188">See also</span></span>

- [<span data-ttu-id="7d1ea-189">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7d1ea-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d1ea-190">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="7d1ea-190">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7d1ea-191">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="7d1ea-191">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
