---
title: Criar Usuário
description: Usar esta API para criar um novo Usuário.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c94c392b009dd2551a97f00ebfe2aa49f7f05db7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278698"
---
# <a name="create-user"></a><span data-ttu-id="12fa6-103">Criar Usuário</span><span class="sxs-lookup"><span data-stu-id="12fa6-103">Create User</span></span>

<span data-ttu-id="12fa6-p101">Crie um novo [usuário](../resources/user.md). O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="12fa6-108">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="12fa6-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12fa6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="12fa6-109">Permissions</span></span>

<span data-ttu-id="12fa6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fa6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12fa6-112">Permission type</span></span>      | <span data-ttu-id="12fa6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12fa6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12fa6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12fa6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="12fa6-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12fa6-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12fa6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12fa6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fa6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fa6-117">Not supported.</span></span>    |
|<span data-ttu-id="12fa6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12fa6-118">Application</span></span> | <span data-ttu-id="12fa6-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fa6-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12fa6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12fa6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="12fa6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12fa6-121">Request headers</span></span>

| <span data-ttu-id="12fa6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12fa6-122">Header</span></span>       | <span data-ttu-id="12fa6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="12fa6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12fa6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12fa6-124">Authorization</span></span>  | <span data-ttu-id="12fa6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12fa6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12fa6-127">Content-Type</span></span>  | <span data-ttu-id="12fa6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12fa6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12fa6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12fa6-129">Request body</span></span>

<span data-ttu-id="12fa6-130">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="12fa6-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="12fa6-131">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="12fa6-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="12fa6-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="12fa6-132">Parameter</span></span> | <span data-ttu-id="12fa6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="12fa6-133">Type</span></span> | <span data-ttu-id="12fa6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="12fa6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12fa6-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="12fa6-135">accountEnabled</span></span> |<span data-ttu-id="12fa6-136">booliano</span><span class="sxs-lookup"><span data-stu-id="12fa6-136">boolean</span></span> |<span data-ttu-id="12fa6-137">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="12fa6-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="12fa6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="12fa6-138">displayName</span></span> |<span data-ttu-id="12fa6-139">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-139">string</span></span> |<span data-ttu-id="12fa6-140">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="12fa6-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="12fa6-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="12fa6-141">onPremisesImmutableId</span></span> |<span data-ttu-id="12fa6-142">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-142">string</span></span> |<span data-ttu-id="12fa6-143">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="12fa6-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="12fa6-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="12fa6-144">mailNickname</span></span> |<span data-ttu-id="12fa6-145">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-145">string</span></span> |<span data-ttu-id="12fa6-146">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="12fa6-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="12fa6-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="12fa6-147">passwordProfile</span></span>|[<span data-ttu-id="12fa6-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="12fa6-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="12fa6-149">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="12fa6-149">The password profile for the user.</span></span>|
|<span data-ttu-id="12fa6-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12fa6-150">userPrincipalName</span></span> |<span data-ttu-id="12fa6-151">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-151">string</span></span> |<span data-ttu-id="12fa6-152">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="12fa6-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="12fa6-153">Como o recurso de **usuário** dá suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="12fa6-153">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="12fa6-154">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="12fa6-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="12fa6-155">Para obter mais informações sobre como alterar isso, confira [exceções para vidas úteis de token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="12fa6-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="12fa6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fa6-156">Response</span></span>

<span data-ttu-id="12fa6-157">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12fa6-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fa6-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12fa6-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12fa6-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12fa6-159">Request</span></span>

<span data-ttu-id="12fa6-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12fa6-160">Here is an example of the request.</span></span>
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

<span data-ttu-id="12fa6-161">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="12fa6-161">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="12fa6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fa6-162">Response</span></span>

<span data-ttu-id="12fa6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="12fa6-166">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="12fa6-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12fa6-167">C#</span><span class="sxs-lookup"><span data-stu-id="12fa6-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12fa6-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="12fa6-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12fa6-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12fa6-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_user_from_users-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
