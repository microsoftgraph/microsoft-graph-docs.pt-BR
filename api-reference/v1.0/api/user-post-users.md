---
title: Criar Usuário
description: Usar esta API para criar um novo Usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46d524c6a3612625c11e5e3d82d283794ab24d99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026625"
---
# <a name="create-user"></a><span data-ttu-id="2faf7-103">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="2faf7-103">Create User</span></span>

<span data-ttu-id="2faf7-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="2faf7-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="2faf7-108">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="2faf7-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2faf7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2faf7-109">Permissions</span></span>

<span data-ttu-id="2faf7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2faf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2faf7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2faf7-112">Permission type</span></span>      | <span data-ttu-id="2faf7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2faf7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2faf7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2faf7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2faf7-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2faf7-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2faf7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2faf7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2faf7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2faf7-117">Not supported.</span></span>    |
|<span data-ttu-id="2faf7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2faf7-118">Application</span></span> | <span data-ttu-id="2faf7-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2faf7-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2faf7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2faf7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="2faf7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2faf7-121">Request headers</span></span>

| <span data-ttu-id="2faf7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2faf7-122">Header</span></span>       | <span data-ttu-id="2faf7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2faf7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2faf7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2faf7-124">Authorization</span></span>  | <span data-ttu-id="2faf7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2faf7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2faf7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2faf7-127">Content-Type</span></span>  | <span data-ttu-id="2faf7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2faf7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2faf7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2faf7-129">Request body</span></span>

<span data-ttu-id="2faf7-130">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2faf7-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="2faf7-131">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="2faf7-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="2faf7-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2faf7-132">Parameter</span></span> | <span data-ttu-id="2faf7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2faf7-133">Type</span></span> | <span data-ttu-id="2faf7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2faf7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2faf7-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="2faf7-135">accountEnabled</span></span> |<span data-ttu-id="2faf7-136">booliano</span><span class="sxs-lookup"><span data-stu-id="2faf7-136">boolean</span></span> |<span data-ttu-id="2faf7-137">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="2faf7-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="2faf7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2faf7-138">displayName</span></span> |<span data-ttu-id="2faf7-139">string</span><span class="sxs-lookup"><span data-stu-id="2faf7-139">string</span></span> |<span data-ttu-id="2faf7-140">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="2faf7-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="2faf7-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="2faf7-141">onPremisesImmutableId</span></span> |<span data-ttu-id="2faf7-142">string</span><span class="sxs-lookup"><span data-stu-id="2faf7-142">string</span></span> |<span data-ttu-id="2faf7-143">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="2faf7-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="2faf7-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2faf7-144">mailNickname</span></span> |<span data-ttu-id="2faf7-145">string</span><span class="sxs-lookup"><span data-stu-id="2faf7-145">string</span></span> |<span data-ttu-id="2faf7-146">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2faf7-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="2faf7-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="2faf7-147">passwordProfile</span></span>|[<span data-ttu-id="2faf7-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="2faf7-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="2faf7-149">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="2faf7-149">The password profile for the user.</span></span>|
|<span data-ttu-id="2faf7-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2faf7-150">userPrincipalName</span></span> |<span data-ttu-id="2faf7-151">string</span><span class="sxs-lookup"><span data-stu-id="2faf7-151">string</span></span> |<span data-ttu-id="2faf7-152">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2faf7-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="2faf7-153">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="2faf7-153">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="2faf7-154">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="2faf7-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="2faf7-155">Para obter mais informações sobre como alterar isso, confira [exceções para vidas úteis de token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="2faf7-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="2faf7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2faf7-156">Response</span></span>

<span data-ttu-id="2faf7-157">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2faf7-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2faf7-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2faf7-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2faf7-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2faf7-159">Request</span></span>

<span data-ttu-id="2faf7-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2faf7-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2faf7-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="2faf7-161">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2faf7-162">C#</span><span class="sxs-lookup"><span data-stu-id="2faf7-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2faf7-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="2faf7-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2faf7-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2faf7-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2faf7-165">Java</span><span class="sxs-lookup"><span data-stu-id="2faf7-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2faf7-166">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2faf7-166">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2faf7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2faf7-167">Response</span></span>

<span data-ttu-id="2faf7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2faf7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
