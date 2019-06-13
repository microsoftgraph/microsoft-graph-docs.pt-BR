---
title: Criar Usuário
description: Usar esta API para criar um novo Usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f023c8882600952feeacffea62b90dc167cf58a
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914683"
---
# <a name="create-user"></a><span data-ttu-id="b9280-103">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="b9280-103">Create User</span></span>

<span data-ttu-id="b9280-p101">Crie um novo usuário. O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="b9280-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="b9280-108">Usuários externos devem ser criados por meio de um convite.</span><span class="sxs-lookup"><span data-stu-id="b9280-108">External users must be created through an invitation.</span></span> <span data-ttu-id="b9280-109">Se você precisar habilitar a criação de usuários externos, consulte [convite](../resources/invitation.md).</span><span class="sxs-lookup"><span data-stu-id="b9280-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9280-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9280-110">Permissions</span></span>

<span data-ttu-id="b9280-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9280-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9280-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9280-113">Permission type</span></span>      | <span data-ttu-id="b9280-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9280-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9280-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9280-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b9280-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9280-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9280-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9280-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9280-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9280-118">Not supported.</span></span>    |
|<span data-ttu-id="b9280-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9280-119">Application</span></span> | <span data-ttu-id="b9280-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9280-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9280-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9280-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="b9280-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9280-122">Request headers</span></span>

| <span data-ttu-id="b9280-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9280-123">Header</span></span>       | <span data-ttu-id="b9280-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9280-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9280-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9280-125">Authorization</span></span>  | <span data-ttu-id="b9280-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9280-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9280-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9280-128">Content-Type</span></span>  | <span data-ttu-id="b9280-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b9280-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9280-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9280-130">Request body</span></span>

<span data-ttu-id="b9280-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b9280-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="b9280-132">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="b9280-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="b9280-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9280-133">Parameter</span></span> | <span data-ttu-id="b9280-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9280-134">Type</span></span> | <span data-ttu-id="b9280-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9280-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9280-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b9280-136">accountEnabled</span></span> |<span data-ttu-id="b9280-137">booliano</span><span class="sxs-lookup"><span data-stu-id="b9280-137">boolean</span></span> |<span data-ttu-id="b9280-138">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="b9280-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="b9280-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b9280-139">displayName</span></span> |<span data-ttu-id="b9280-140">string</span><span class="sxs-lookup"><span data-stu-id="b9280-140">string</span></span> |<span data-ttu-id="b9280-141">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9280-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="b9280-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="b9280-142">onPremisesImmutableId</span></span> |<span data-ttu-id="b9280-143">string</span><span class="sxs-lookup"><span data-stu-id="b9280-143">string</span></span> |<span data-ttu-id="b9280-144">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9280-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="b9280-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b9280-145">mailNickname</span></span> |<span data-ttu-id="b9280-146">string</span><span class="sxs-lookup"><span data-stu-id="b9280-146">string</span></span> |<span data-ttu-id="b9280-147">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9280-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="b9280-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="b9280-148">passwordProfile</span></span>|[<span data-ttu-id="b9280-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="b9280-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="b9280-150">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9280-150">The password profile for the user.</span></span>|
|<span data-ttu-id="b9280-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9280-151">userPrincipalName</span></span> |<span data-ttu-id="b9280-152">string</span><span class="sxs-lookup"><span data-stu-id="b9280-152">string</span></span> |<span data-ttu-id="b9280-153">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b9280-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="b9280-154">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="b9280-154">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="b9280-155">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="b9280-155">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="b9280-156">Para obter mais informações sobre como alterar isso, confira [exceções para vidas úteis de token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="b9280-156">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="b9280-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9280-157">Response</span></span>

<span data-ttu-id="b9280-158">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9280-158">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9280-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9280-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9280-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9280-160">Request</span></span>

<span data-ttu-id="b9280-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9280-161">Here is an example of the request.</span></span>
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

<span data-ttu-id="b9280-162">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b9280-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b9280-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9280-163">Response</span></span>

<span data-ttu-id="b9280-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9280-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="b9280-167">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b9280-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9280-168">C#</span><span class="sxs-lookup"><span data-stu-id="b9280-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9280-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9280-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
