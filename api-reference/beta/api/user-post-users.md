---
title: Criar usuário
description: Crie um novo usuário.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 56c2259c74ebdec363c49c30d781a1a891a08b0e
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080813"
---
# <a name="create-user"></a><span data-ttu-id="d8ae8-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="d8ae8-103">Create user</span></span>

<span data-ttu-id="d8ae8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ae8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8ae8-105">Create a new [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-105">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="d8ae8-106">The request body contains the user to create.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-106">The request body contains the user to create.</span></span> <span data-ttu-id="d8ae8-107">At a minimum, you must specify the required properties for the user.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-107">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="d8ae8-108">You can optionally specify any other writable properties.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-108">You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="d8ae8-109">Essa operação retorna, por padrão, apenas um subconjunto das propriedades de cada usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-109">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="d8ae8-110">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-110">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="d8ae8-111">Para obter propriedades não retornadas por padrão, execute uma [operação GET](user-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-111">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="d8ae8-112">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-112">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8ae8-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8ae8-113">Permissions</span></span>

<span data-ttu-id="d8ae8-114">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-114">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d8ae8-115">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-115">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ae8-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8ae8-116">Permission type</span></span>      | <span data-ttu-id="d8ae8-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8ae8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8ae8-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8ae8-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d8ae8-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8ae8-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8ae8-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8ae8-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8ae8-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-121">Not supported.</span></span>    |
|<span data-ttu-id="d8ae8-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8ae8-122">Application</span></span> | <span data-ttu-id="d8ae8-123">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ae8-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8ae8-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ae8-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="d8ae8-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ae8-125">Request headers</span></span>
| <span data-ttu-id="d8ae8-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8ae8-126">Header</span></span>       | <span data-ttu-id="d8ae8-127">Valor</span><span class="sxs-lookup"><span data-stu-id="d8ae8-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8ae8-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8ae8-128">Authorization</span></span>  | <span data-ttu-id="d8ae8-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-129">Bearer {token}.</span></span> <span data-ttu-id="d8ae8-130">Required.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-130">Required.</span></span>  |
| <span data-ttu-id="d8ae8-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8ae8-131">Content-Type</span></span>  | <span data-ttu-id="d8ae8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ae8-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8ae8-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ae8-133">Request body</span></span>

<span data-ttu-id="d8ae8-134">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-134">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="d8ae8-135">A tabela a seguir lista as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-135">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="d8ae8-136">Se você estiver incluindo uma propriedade de **identidades** para o usuário que está criando, nem todas as propriedades listadas serão necessárias.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-136">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="d8ae8-137">Para obter uma [identidade de conta local B2C](../resources/objectidentity.md), só é necessário **passwordProfile** e **passwordPolicy** deve ser definido como `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-137">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="d8ae8-138">Para uma identidade social, nenhuma das propriedades é necessária.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-138">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="d8ae8-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8ae8-139">Parameter</span></span> | <span data-ttu-id="d8ae8-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8ae8-140">Type</span></span> | <span data-ttu-id="d8ae8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8ae8-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8ae8-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="d8ae8-142">accountEnabled</span></span> |<span data-ttu-id="d8ae8-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8ae8-143">Boolean</span></span> |<span data-ttu-id="d8ae8-144">True se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-144">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="d8ae8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d8ae8-145">displayName</span></span> |<span data-ttu-id="d8ae8-146">string</span><span class="sxs-lookup"><span data-stu-id="d8ae8-146">string</span></span> |<span data-ttu-id="d8ae8-147">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-147">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="d8ae8-148">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="d8ae8-148">onPremisesImmutableId</span></span> |<span data-ttu-id="d8ae8-149">string</span><span class="sxs-lookup"><span data-stu-id="d8ae8-149">string</span></span> |<span data-ttu-id="d8ae8-150">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-150">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="d8ae8-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d8ae8-151">mailNickname</span></span> |<span data-ttu-id="d8ae8-152">string</span><span class="sxs-lookup"><span data-stu-id="d8ae8-152">string</span></span> |<span data-ttu-id="d8ae8-153">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-153">The mail alias for the user.</span></span>|
|<span data-ttu-id="d8ae8-154">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d8ae8-154">passwordProfile</span></span>|[<span data-ttu-id="d8ae8-155">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="d8ae8-155">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="d8ae8-156">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-156">The password profile for the user.</span></span>|
|<span data-ttu-id="d8ae8-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8ae8-157">userPrincipalName</span></span> |<span data-ttu-id="d8ae8-158">string</span><span class="sxs-lookup"><span data-stu-id="d8ae8-158">string</span></span> |<span data-ttu-id="d8ae8-159">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-159">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="d8ae8-160">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-160">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="d8ae8-161">Os usuários federados criados por meio dessa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-161">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="d8ae8-162">Para obter informações sobre como alterar isso, confira [exceções para tempos de vida do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-162">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="d8ae8-163">A adição de uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente não é permitida, a menos que o objeto **User** já contenha uma identidade de conta local.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-163">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="d8ae8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ae8-164">Response</span></span>

<span data-ttu-id="d8ae8-165">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-165">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ae8-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8ae8-166">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="d8ae8-167">Exemplo 1: criar um usuário</span><span class="sxs-lookup"><span data-stu-id="d8ae8-167">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="d8ae8-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ae8-168">Request</span></span>
<span data-ttu-id="d8ae8-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-169">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8ae8-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ae8-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8ae8-171">C#</span><span class="sxs-lookup"><span data-stu-id="d8ae8-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8ae8-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8ae8-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8ae8-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8ae8-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d8ae8-174">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d8ae8-174">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d8ae8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ae8-175">Response</span></span>
<span data-ttu-id="d8ae8-176">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-176">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="d8ae8-177">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-177">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8ae8-178">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-178">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="d8ae8-179">Exemplo 2: criar um usuário com identidades de conta social e local</span><span class="sxs-lookup"><span data-stu-id="d8ae8-179">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="d8ae8-180">Crie um novo usuário, com uma identidade de conta local, com um nome de logon, um endereço de email como logon e com uma identidade social.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-180">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="d8ae8-181">Esse exemplo é geralmente usado para cenários de migração em locatários de B2C.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-181">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="d8ae8-182">Para as identidades de conta local, as expirações de senha devem ser desabilitadas e forçar alteração de senha no próximo logon também deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-182">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="d8ae8-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ae8-183">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d8ae8-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ae8-184">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8ae8-185">C#</span><span class="sxs-lookup"><span data-stu-id="d8ae8-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8ae8-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8ae8-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8ae8-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8ae8-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d8ae8-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ae8-188">Response</span></span>

<span data-ttu-id="d8ae8-189">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-189">Here is an example of the response.</span></span> 

> <span data-ttu-id="d8ae8-190">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8ae8-191">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d8ae8-191">All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d8ae8-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8ae8-192">See also</span></span>

- [<span data-ttu-id="d8ae8-193">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d8ae8-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d8ae8-194">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="d8ae8-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d8ae8-195">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="d8ae8-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
